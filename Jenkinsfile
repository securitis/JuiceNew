pipeline {
  agent any 
     
        
  tools {
    maven 'maven'
  }
        
  environment {
    Snyk = 'Snyk'
    Trivy = 'Trivy'
    Audit = 'Audit'
  }
  
  stages {
    stage ('Initialize') {
      steps {
        sh '''
                    echo "PATH = ${PATH}"
                    echo "M2_HOME = ${M2_HOME}"
                  
            ''' 
      }
    } 
    
     
 stage ('CxOne Jenkins Scan') {
      steps {
        sh 'sudo chmod 666 /var/run/docker.sock'
        //sh 'sudo docker run raphaelareya/gitleaks:latest -r https://github.com/securitis/CICD.git'       
        //sh 'rm trufflehog || true'
        //sh 'docker run gesellix/trufflehog --json https://github.com/cehkunal/webapp.git > trufflehog'
        //sh 'cat trufflehog'
      }
    }  
         
 
    
  }
} 



