pipeline {
    agent any

    stages {
        // Here I assign different stages for Jenkins 
        stage("build") {
            steps {
                // In my case as it is javascript application i will run here commands like:
                // sh 'npm install' 
                // sh 'npm build'
                echo 'building the application...'
            }
        }
        stage("test") {
            steps {
                echo 'testing the application...'
                
            }
        }
        stage("deploy") {
            steps {
                echo 'deploying the application...'
                
            }
        }
    }
}