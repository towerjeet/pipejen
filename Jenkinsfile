pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh (chmod 777 ./jenkins/build/mvn.sh mvn -B -DskipTests clean package);
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
