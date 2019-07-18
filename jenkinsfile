pipeline {
    agent { label 'master' }
    stages {
        stage('git_clone_demo') {
            steps {
                echo 'Hello world!' 
                git 'https://github.com/kolimikeshava/kesava.git'
            }
        }
    stage('Build') {
        steps {
            echo 'helloword'
            sh '''
            mvn clean
            mvn compile
            mvn test
            mvn package
            '''
        }
    }
    stage('shell') {
        steps {
            sh '''mkdir reddy
            cd reddy
            touch file1'''
        }
    }
       }
}
