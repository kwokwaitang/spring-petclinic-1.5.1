pipeline {
    agent {
        docker {
            image 'maven:3.5.0'
        }
    }
    stages {
        stage('Maven Install') {
            steps {
                echo 'About to do a clean & install'
                sh 'mvn clean install'
            }
        }
    }
}
