pipeline {
    agent Docker
    options {
        skipStagesAfterUnstable()
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        
        // stage 2
        stage('Deploy') {
            steps {
                echo 'Deploying..'
            }
        }
        stage('ValidateStageDeployment') {
            steps {
                echo 'validate deployment on staging....'
            }
        }
    }
}
