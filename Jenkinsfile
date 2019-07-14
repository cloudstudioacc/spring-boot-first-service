pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                   echo 'This is a minimal pipeline.'
            }
        }

        stage ('Testing Stage') {

            steps {
                    echo 'This is a minimal pipeline.'
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