pipeline {
  
  agent { node { label 'master' } }
  
  parameters {
    string(name: 'filename', defaultValue: '', description: 'Please enter file name') 
    choice(name: 'filelist', choices: ['handy', 'hearty', 'smurfet'], description: 'Choose a file')
  }
         
  stages {
    stage ('print handy content') {
           steps {
               sh 'cat handy.txt'
           }
     }      
    
    stage ('print hearty content') {
           steps {
             sh "cat ${params.filename}"
           }
     }
    
     stage ('print from choice') {
           steps {
             sh "cat ${params.filelist}.txt"
           }
     }
    
   }
                
}
