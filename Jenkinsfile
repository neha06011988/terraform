pipeline {
    agent any
    stages {
        stage("Initializing Phase") {
            steps {
            sh "sudo apt-get update"
            sh "scrip.sh"
            sh "Terraform init"
            }
        }
        stage("Planing Phase") {
            steps {
            sh "Terraform plan"
            }
        }
        stage("Apply Phase") {
            steps {
            sh "Terraform apply"
            }
        }
    }
    
}
