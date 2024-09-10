pipeline {
    agent {
        label 'Slave-01'
    }
    
    tools{
        jdk 'java17'
        maven 'maven3'
    }

    stages {
        stage('Git CheckOut') {
            steps {
                git branch: 'test', url: 'https://github.com/Raghava0684/Petclinic-project.git'
            }
        }
        
        stage('Compile') {
            steps {
               sh "mvn clean compile"
            }
        }
        
        stage('Clean Package') {
            steps {
                sh "mvn clean package -DskipTests=true"
            }
        }
    }
}
