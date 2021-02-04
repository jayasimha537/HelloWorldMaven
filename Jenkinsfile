pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                srcipt{
                if (env.GIT_BRANCH == 'origin/master' ) { 
                    echo "Something changed in master branch"
                }
                echo "Hai Jay"
                }
            }
        }
    }
}
