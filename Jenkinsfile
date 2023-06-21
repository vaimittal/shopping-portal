pipeline{

    agent any

// uncomment the following lines by removing /* and */ to enable
    tools{
       nodejs 'nodejs' 
    }
    

    stages{
        stage('Build'){
            steps{
                echo 'this is build the app job'
                sh 'npm install'
            }
        }
        stage('Test'){
            steps{
                echo 'this is test the app job'
                sh 'npm test'
            }
        }
        stage('Package'){
            steps{
                echo 'this is package the app job'
                sh 'npm run package'
            }
        }
    }
    
    post{
        always{
            echo 'Hello...My first pipeline through code...'
        }
        
    }
    
}
