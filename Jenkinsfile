pipeline {  

    agent any
        
    tools{
        maven "maven3"
    }
    stages {
        stage('Clone Repository') {
            steps {
               git 'https://github.com/ashokitschool/maven-web-app.git'
            }
        }
        stage('Build') {
            steps {
               sh 'mvn clean package'
            }
        }
    }
}
