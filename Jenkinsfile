pipeline {
    agent any
    stages {
        stage ('git checkout'){
            steps {
                git 'https://github.com/formycore/valaxy.git'
            }   
        }
        stage ('Mvn compile'){
            steps {
                sh 'mvn compile'
            }
        }
        stage ('Test'){
            steps {
                sh 'mvn test'
            }
        }
        stage ('Clean install'){
            steps {
                sh 'mvn clean install'
            }
        }
    }
}
