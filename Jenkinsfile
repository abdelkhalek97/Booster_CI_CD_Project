pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                
                git url: 'https://github.com/abdelkhalek97/Booster_CI_CD_Project.git' ,branch: 'main'
                sh "ls"

          }
        }
        
        stage ("terraform init") {
            steps {
                
                sh "terraform init"
                sh "terraform plan"
            }
        }
    }
}
