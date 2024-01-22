pipeline {
    agent any
    stages{
     stage('initialize'){
        steps {
            sh 'terraform init'
        }
     }
     stage('format the code'){
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
     stage('apply'){
        stage{
            sh 'terraform apply --auto-approve'
        }
     }
    }
 }
