pipeline {
    agent {
        label 'ansible'
    }
    stages {
        stage('Download role from github') {
            steps {
                git 'https://github.com/kshatyy/vector-role.git'
            }
        }
        stage('m_test') {
            steps {
                sh 'molecule test'
            }
        }
    }
}
