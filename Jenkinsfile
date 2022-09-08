pipeline {
    agent {label 'test_agent'}
    
    stages {
        stage("Licensing") {
            steps {
			    powershell '''
			    echo '"${BRANCH_NAME}"'
			    echo '"${GIT_BRANCH}"'
			    echo '"${env:GIT_BRANCH}"'
			    echo '"${env:BRANCH_NAME}"'
			    echo '"env:BRANCH_NAME"'
			    echo '"env:GIT_BRANCH"'
			    '''
            }
        }
    }
}


