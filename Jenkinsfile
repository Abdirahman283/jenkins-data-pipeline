pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    echo eleve | sudo -S apt update
                    echo eleve | sudo -S apt install -y python3 python3-pip
                    pip3 install pandas
                    python3 data_analysis.py
                '''
            }
        }
    }
}
