pipeline {
  
  agent { node { label 'master' } }
  
  parameters {
   string(name: 'filename', defaultValue: '', description: 'Please enter file name') 
  }
         
  stages {
    stage ('Print handy content') {
           steps {
               sh 'cat handy.txt'
           }
     }      
    
    stage ('Read hearty content') {
           steps {
             sh 'cat ${params.filename}'
           }
       }
    
   }
                
}
