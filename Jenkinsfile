pipeline {
    agent any

    tools {
        maven "MBOC"
        jdk "jdk11"
    }

    stages {
        stage('Build') {
            steps {
                git branch: 'master', url: 'https://github.com/DAlzx/boc-controle.git'
                sh "mvn package"
            }
        }
        stage('coucou') {
            steps {
                sh "echo 'coucou'"
            }
        }
    }
}
