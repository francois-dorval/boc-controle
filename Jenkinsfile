pipeline {
    agent any
    
    tools {
        maven 'MBOC' //  la bonne version de Maven configurée dans Jenkins
        jdk 'jdk11' // la bonne version de Java configurée dans Jenkins
    }
    
    stages {
        stage('Checkout') {
            steps {
                git branch: 'master', // Le nom de la branche souhaitée
                    url: 'https://github.com/Ndouma1/boc-controle.git' // 
            }
        }
        
        stage('Build') {
            steps {
                sh 'mvn clean package' // Exécute la commande Maven pour compiler et construire le projet
            }
        }
        
        // Autres étapes de votre pipeline
    }
}
