pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                sh 'python -m py_compile seed.py' 
                stash(name: 'compiled-results', includes: 'sources/*.py*') 
            }
        }
    }
}