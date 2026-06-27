pipeline {
    agent any
    
    stages {
        stage ('hello-world') {
            steps {
                sh "echo 'hello world from a shell script!'"
            }
        }
        stage ('hello-nti') {
            steps {
                sh '''
                echo "echo hello-nti" > hello-nti.sh
                chmod +x hello-nti.sh
                ./hello-nti.sh
                docker ps 
                '''
            }
        }
    }
}
