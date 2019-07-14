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
                withMaven(maven : '${MAVEN_HOME}') {
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