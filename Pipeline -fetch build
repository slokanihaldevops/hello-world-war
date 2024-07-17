pipeline{
    agent any
    
    environment{
        PATH = "/usr/share/maven/bin/:$PATH"
    }
    stages{
        stage("Git Checkout"){
            steps{
                git 'https://github.com/slokanihaldevops/hello-world-war.git'
            }
        }
        stage("Maven Build"){
            steps{
                sh "mvn clean package"
            }
        }
       
        }
    }
