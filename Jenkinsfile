pipeline{
    stage('Checkout'){
        git branch: 'main', url:'https://github.com/pillaiuma/SpringPetClinic.git'
    }
    stage('Build'){
        withMaven(maven: 'M3'){
            bat 'mvn compile'
        }
    }
}
