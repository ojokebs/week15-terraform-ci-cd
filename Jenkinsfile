pipeline {
    agent any
    stages{
     stage('init'){
        steps {
            sh 'terraform init'
        }
     }
     stage('format'){
        steps{
            sh 'terraform fmt'
        }
     }
     stage('validate'){
        stage{
            sh 'terraform validate'
        }
     }
     stage('plan'){
        stage{
            sh 'terraform plan'
        }
     }
     stage('destroy'){
        stage{
            sh 'terraform destroy --auto-approve'
        }
     }
    }
 }
