pipeline {
  agent { node { label 'master' } }
         
  stages {
    stage ('Print handy content') {
           steps {
               sh 'cat handy.txt'
           }
     }      
    
    stage ('Read smurfet content') {
           steps {
              sh 'cat smurfet.txt'
           }
       }
    
   }
                
}
