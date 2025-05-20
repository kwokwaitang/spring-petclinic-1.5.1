pipeline {
    agent none
    stages {
        stage('Maven Install') {
            echo 'Running agent for maven:3.5.0'
            agent {
                docker {
                    image 'maven:3.5.0'
                }
            }
            steps {
                echo 'About to do a clean & install'
                sh 'mvn clean install'
            }
        }
    }
}
