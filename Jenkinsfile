pipeline {
    agent any

    
    stages {
        stage('Login and Push'){
            steps {
                script{
                    withDockerRegistry(credentialsId: 'js7117') {
                        docker.build('js7117/flaskapp').push('latest')
                    }
                }
            }
        }
    }
}