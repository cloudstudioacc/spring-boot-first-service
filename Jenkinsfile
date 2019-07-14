pipeline {
    agent any

    stages {
        stage ('Description Stage') {

            steps {
                    sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                    echo "MAVEN_HOME=${MAVEN_HOME}"
                ''' 
            }
        }

        stage ('Compile Stage') {

            steps {
                withMaven(maven : '/Users/yaserarafatmohammad/dev/apache-maven-3.3.9/bin') {
                    sh 'mvn clean compile'
                }
            }
        }


        stage ('Deployment Stage') {
            steps {
                    sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                ''' 
            }
        }
    }
}