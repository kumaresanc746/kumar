pipeline {
    agent any
 
    stages {
        stage('build') {
            steps {
                sh 'mkdir -p ${WORKSPACE}/my-app'
                sh 'cp -r /home/ubuntu/my-app/* ${WORKSPACE}/my-app/'
                dir('my-app') {
                    sh 'mvn clean install'
                }
            }
        }
 
        stage('test') {
            steps {
                echo 'Hi Good'
            }
        }
 
        stage('deploy') {
            steps {
                echo 'Hi Everyone'
            }
        }
    }
}
