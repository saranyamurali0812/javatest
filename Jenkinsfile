pipeline {
       agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy uat') {
            steps {
                echo 'Deploying FILE....'
            }
        }
         stage('Deploy pre prod') {
            steps {
                echo 'stagging....'
            }
        }
         stage('prod approval') {
            steps {
               script{
                if (env.BRANCH_NAME == "feature-txt"){
                    input('proceed for prod deployment ')
                }
               }
            }
        }
    }
}