pipeline { 
  
   agent any

   stages {
   
     stage('Pulling git code') { 
        steps { 
           git credentialsId: 'admin', url: 'https://github.com/sowmyarajgit/test-nodejs-app.git'
        }
     }
     
     stage('install dependencies') { 
        steps { 
           sh 'npm install'
        }
      }

         stage("nodejs build") { 
         steps { 
           sh 'npm build'
         }

     }
  
   	}

   }
