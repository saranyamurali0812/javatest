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
        stage('Deploy to uat') {
            steps {
                echo 'Deploying FILE....'
            }
        }
         stage('Deploy to prod') {
            steps {
                echo 'Deploying prod file....'
            }
        }
         stage('prod approval') {
            steps {
               if (ENV.BRANCH_NAME == "master"){
                input('proceed for prod deployment ?')
               }
            }
        }
    }
}