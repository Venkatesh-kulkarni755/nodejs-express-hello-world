
pipeline {
    agent any
    
   
    stages {
        stage("clean") {
            steps {
                sh "rm -rf nodejs-express-hello-world"
            }
        }
        stage("clone"){
            steps {
            
                sh "git clone https://github.com/Venkatesh-kulkarni755/nodejs-express-hello-world.git "
            

            }
        }
        
        stage('build') {
            steps {
                
                sh '''
                    cd nodejs-express-hello-world
                    docker build -t demo:jenkins .
                '''
        }
        
       
    }
}
