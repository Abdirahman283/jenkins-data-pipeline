pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'echo eleve | sudo -S apt update'  // mise a jour du dep>
                    sh 'echo eleve | sudo -S apt install -y python3 python3-pip'
                    sh 'pip3 install pandas' // Installer les dépendances
                    sh 'python3 data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}
