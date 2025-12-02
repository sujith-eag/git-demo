pipeline {
    agent any

    stages {
        stage('Branch Based Echo') {
            steps {
                script {
                    def branch = env.BRANCH_NAME

                    echo "Current branch: ${branch}"

                    if (branch == "main") {
                        echo "Running steps for MAIN branch"
                    }
                    else if (branch == "dev") {
                        echo "Running steps for DEVELOP branch"
                    }
                    else {
                        echo "Running steps for OTHER branches"
                    }
                }
            }
        }
    }
}
