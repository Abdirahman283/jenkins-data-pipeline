pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                script {
                    sh 'pip install pandas' // Installer les dépendances
                    sh 'python data_analysis.py' // Exécuter le script Python
                }
            }
        }
    }
}
