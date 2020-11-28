pipeline{
    tools{
        maven 'Maven 3'
        jdk 'java11'
    }
    agent{
        label 'maven'
    }
    stages{
        stage('checkout'){
            steps{
                 git 'https://github.com/VinYuvian/JavaDevops.git'
            }
        }
    
        stage('compile'){
            steps{
                //echo "${PATH}"
                sh 'mvn compile'
                //mvn compile
            }
            
        }
        
        stage('test'){
            steps{
                //echo "${M2_HOME}"
                sh 'mvn verify'
                //mvn verify
            }
            
        }
    }
}