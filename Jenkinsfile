pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage ('Ejemplo shell script') {
            agent { label 'docker-agent' }
            steps {
                sh """
                   hostname
                   ls -la
                   pwd
                """
            }
        }
    }
}
