pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('build-the-app'){
            steps{
                echo 'this is the first job'
                sh 'npm install'
         //       sleep 4
            }
        }
        stage('two'){
            steps{
                echo 'this is the second job'
                sh 'npm test'
         //       sleep 9
            }
        }
        stage('three'){
            steps{
                echo 'this is the third job'
                sh 'npm run package'
         //       sleep 7
            }
        }
    }
    
    post{
        always{
            echo 'this pipeline has completed...'
        }
        
    }
    
}
