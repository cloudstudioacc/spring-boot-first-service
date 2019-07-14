pipeline {
    agent any
    tools {
        maven '/opt/maven/apache-maven-3.6.1' 
    }
    stages {
        stage('Example') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}