pipeline {
    agent any 
    stages {
        stage('master') { 
            steps {
                echo 'Taking code fron Git hub' 
                git "https://github.com/jfrog/project-examples.git/"
                echo 'code taken'
            }
        }
        stage('build') { 
            steps {
                echo 'creating text file'
                writeFile file: 'demo.txt',text: 'Working with files the Groovy way is easy.'
            }
        }
        stage('Deploy') { 
            steps {
                echo 'deploying to container' 
            }
        }
    }
}
