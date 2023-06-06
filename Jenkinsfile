pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                git branch: 'main', url: 'https://github.com/chaeyeon-demo/jenkins_demo.git'
            }
        }
        stage('mvn') {
            steps {
                bat "mvn -Dmaven.test.failure.ignore=true clean test"
            }
        }
    }
}
