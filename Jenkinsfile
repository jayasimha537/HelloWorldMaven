pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                srcipt{
                if (env.GIT_BRANCH == 'origin/master' && env.ghprbSourceBranch == null ) { 
                    echo "Something changed in master branch"
                }
                
                if  (env.ghprbSourceBranch != null ) { 
                    echo "PR has been raised"
                    echo "Soruce branch: ${env.ghprbSourceBranch}"
                }
                
                echo "Hai Jay"
                }
            }
        }
    }
}
