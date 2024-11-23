pipeline{
    agent any
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
                sh 'npm install'
                sh 'npm run test'
            }
        }

        stage('package'){ //include archiving artifact
            steps{
                sh'npm install'
                sh 'npm run package'
            }
        }
    }

    tools{
        nodejs 'NodeJS 4.8.6'
    }
}