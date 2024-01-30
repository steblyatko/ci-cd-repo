pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }

        stage('Notification') {
            steps {
                emailext body: 'Test Message',
                    subject: 'Test Subject',
                    to: 'mega.steblyatko@gmail.com'
            }
        }
    }
}