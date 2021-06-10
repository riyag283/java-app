pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                bat "javac App.java"
                bat "java App abcd"
            }
        }
    }
}