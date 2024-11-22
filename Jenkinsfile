pipeline{
    agent any
    tools{

    }
    //look at package.json for npm scripts
    stages{
        stage('build'){//npm install
            steps{
                sh 'npm install'
                sh 'npm run build'
            }
        }

        stage('test'){
            steps{
                sh 'npm run test'

            }
        }

        stage('package'){ //include archiving artifact
            steps{
                sh 'npm run package'
                sh 'npm run postpackage'
            }
        }
    }
}