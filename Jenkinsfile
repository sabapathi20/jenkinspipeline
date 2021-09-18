pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'This is build phase'
            }
        
            }

            post {
                always {
                    junit '**/target/surefire-reports/TEST-*.xml'
                }
            }
        }
    
}
