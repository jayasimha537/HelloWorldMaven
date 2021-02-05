pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                
                echo "x=100"
                script { 
                    if (env.GIT_BRANCH == 'origin/master' && env.ghprbSourceBranch == null ) {
                                echo 'Something changed in master'
                            }
                    if (env.GIT_BRANCH == 'origin/master' && env.ghprbSourceBranch != null ) {
                        echo "PR has been raised from ${env.ghprbSourceBranch}"
                            } 
                        }
            }
        }
    }
}
