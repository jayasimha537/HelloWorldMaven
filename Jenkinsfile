pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh 'printenv'
                echo "Hai Jay"
                script { 
                    if (env.BRANCH_NAME == 'master' ) {
                        echo 'Something changed in master'
                            } 
                        }
            }
        }
    }
}
