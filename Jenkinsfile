pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
            git url: 'https://github.com/abdelkhalek97/Booster_CI_CD_Project.git' ,branch: 'main'

          }
        }
        
        stage ("terraform init") {
            steps {
                sh "terraform init" 
            }
        }
        
        stage ("terraform Action") {
            steps {
                sh "echo "Terraform action is --> ${action}""
                sh "terraform ${action} --auto-approve"
           }
        }
    }
}
