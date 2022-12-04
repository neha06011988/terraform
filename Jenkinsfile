pipeline {
    agent any
    stages {
        stage("Initializing Phase") {
            steps {
            sh "sudo apt-get update"
            sh "terraform init"
            }
        }
        stage("Planing Phase") {
            steps {
            sh "terraform plan"
            }
        }
        stage("Apply Phase") {
            steps {
            sh "terraform apply"
            }
        }
    }
    
}
