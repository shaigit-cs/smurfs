pipeline {
  agent { node { label 'master' } }
         
  stages {
    stage ('Print handy content') {
           steps {
               sh 'cat handy.txt'
           }
     }      
    
    stage ('Read hearty content') {
           steps {
              sh 'cat hearty.txt'
           }
       }
    
   }
                
}
