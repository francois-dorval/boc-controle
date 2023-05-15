pipeline {
    agent any
    
    tools {
        // Spécifiez la version correcte de Maven et du JDK
        maven 'MBOC'
        jdk 'jdk11'
    }
    
    stages {
        stage('Checkout du projet') {
            steps {
                git branch: 'master', url: 'https://github.com/theace97/boc-controle.git'
            }
        }
        
        stage('Build Maven') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
