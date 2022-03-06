pipeline {
  
  agent { node { label 'master' } }
  
  parameters {
    string(name: 'filename', defaultValue: '', description: 'Please enter file name') 
    choice(name: 'filelist', choices: ['handy', 'hearty', 'smurfet'], description: 'Choose a file')
  }
         
  stages {
    stage ('Print handy content') {
           steps {
               sh 'cat handy.txt'
           }
     }      
    
    stage ('Read hearty content') {
           steps {
             sh "cat ${params.filename}"
           }
     }
    
     stage ('Read from choice') {
           steps {
             sh "cat ${params.filelist}.txt"
           }
     }
    
   }
                
}
