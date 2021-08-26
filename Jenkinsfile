pipeline{
    agent{label 'master'}
    tools{maven 'M3'}
    stages{
        stage('Checkout'){
            steps{
                git branch: 'main',url:'https://github.com/pillaiuma/SpringPetClinic.git'
            }
        }
        stage('Build'){
            steps{
                bat 'mvn compile'
            }
        }
        stage('Test'){
            steps{
                bat 'mvn test'
            }
        }
    }
}
