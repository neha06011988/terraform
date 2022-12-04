pipeline {
    agent any
    stages {
        stage("Initializing Phase") {
            steps {
            #sh "gpg --no-default-keyring \ --keyring /usr/share/keyrings/hashicorp-archive-keyring.gpg \ --fingerprint"
            sh "sudo apt-get update"
            sh "sudo apt-get install terraform"
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
