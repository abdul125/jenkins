pipeline {
  agent {
    docker {
      image "bryandollery/terraform-packer-aws-alpine"
      args "-u root --entrypoint=''"
    }

    stages {
        stage('Build') {
            steps {
                'packer build packer.json'
                echo 'building cre..'
            }
        }
        
        // stage 2
        stage('deploying') {
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
