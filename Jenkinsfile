pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh '''
                    sudo -S apt update
                    sudo -S apt install -y python3 python3-pip
                    pip3 install pandas
                    python3 data_analysis.py
                '''
            }
        }
    }
}
