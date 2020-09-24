pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh '''
                      chmod u+x
                    ./jenkins/build/mvn.sh mvn -B -DskipTests clean package
                    chmod u+x
                    ./jenkins/build/build.sh

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
