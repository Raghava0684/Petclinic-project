pipeline {
    agent any
    
    tools {
        jdk 'jdk17'
        maven 'maven3'
    }

    //stages {
        //stage('Git Checkout') {
          //  steps {
           //     git branch: 'prod', url: 'https://github.com/Raghava0684/Petclinic-project.git'
          //  }
      //  }
        
        stage('Mvn compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('Mvn package') {
            steps {
                sh 'mvn package'
            }
        }
    
    }
}
