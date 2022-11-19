pipeline {
    agent none

    stages {
        stage('stage 1') {
            agent {label 'slave1'}
            steps {
                echo 'running on label slave1'
            }
        }
        stage('stage 1-A') {
            agent {label 'master'}
            steps {
                echo 'running on label master'
            }
        }
        stage('stage 2') {
            agent {label 'slave1'}
            steps {
                echo 'running on slave1'
            }
        }
        
    }
}
