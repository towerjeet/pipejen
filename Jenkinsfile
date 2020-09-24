pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                    chmod 777 ./jenkins/build/mvn.sh mvn -B -DskipTests clean package
                    chmod 777 ./jenkins/build/build.sh

                '''
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
