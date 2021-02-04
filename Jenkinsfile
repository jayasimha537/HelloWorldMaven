pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                sh 'printenv'
                echo "Hai Jay"
                script { 
                    if (env.GIT_BRANCH == 'origin/master' && env.ghprbSourceBranch == null ) {
                                echo 'Something changed in master'
                            }
                    if (env.GIT_BRANCH == 'origin/master' && env.ghprbSourceBranch != null ) {
                                echo 'PR has been raised'
                            } 
                        }
            }
        }
    }
}
