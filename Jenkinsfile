pipeline {
    agent {label 'test_agent'}
    
    stages {
	    stage("GitCheckout") {
	    	steps {
			git branch: 'main', credentialsId: '95ae0d33-6c92-4b9e-b08e-bc3d0cccc12b', url: 'https://github.com/devsecops09/demo.git'
		}
    }
	    stage("Licensing") {
            	steps {
			    powershell '''
			    # echo "${BRANCH_NAME}"
			    # echo "${GIT_BRANCH}"
			    echo "${env:GIT_BRANCH}"
			    # echo "${env:BRANCH_NAME}"
			    # echo "env:BRANCH_NAME"
			    # echo "env:GIT_BRANCH"
			    '''
            }
        }
    }
}


