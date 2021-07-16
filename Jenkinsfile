pipeline{
    agent{label 'master'}
    tools{maven 'M3'}
    stages{
        stage('checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/Nage4455/SpringPetClinic.git'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('Test'){
            steps{
                sh  'mvn test'
            }
        }
        stage('package'){
            steps{
                sh 'mvn package'
            }
            
        }
        stage('Deploy'){
            steps{
                sh 'java -jar /var/lib/jenkins/workspace/PetClinicDeclarative pipeline/*.jar'
            }
        }
    }
}pipeline{
    agent{label 'master'}
    tools{maven 'M3'}
    stages{
        stage('checkout'){
            steps{
                git branch: 'main', url: 'https://github.com/Nage4455/SpringPetClinic.git'
            }
        }
        stage('Build'){
            steps{
                sh 'mvn compile'
            }
        }
        stage('Test'){
            steps{
                sh  'mvn test'
            }
        }
        stage('package'){
            steps{
                sh 'mvn package'
            }
            
        }
        stage('Deploy'){
            steps{
                sh 'java -jar /var/lib/jenkins/workspace/PetClinicDeclarativepipeline/*.jar'
            }
        }
    }
}
