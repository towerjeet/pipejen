pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh  "chmod +x -R /var/jenkins_home/workspace/devops"
                sh  "./jenkins/build/mvn.sh mvn -B -DskipTests clean package"
                sh "./jenkins/build/build.sh"
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
