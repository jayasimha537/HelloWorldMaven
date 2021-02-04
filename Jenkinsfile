pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh 'printenv'
                echo "Hai Jay"
                script { 
                    if (env.GIT_BRANCH == 'origin/master' ) {
                        echo 'Something changed in master'
                            } 
                        }
            }
        }
    }
}
