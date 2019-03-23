pipeline {
    agent any
    tools {
        maven 'maven-3.6.0' 
          }
    stages 
    {
        stage('compile')
          {
            steps {
                sh 'mvn clean compile'
                  }
           }
    
        
    }
}
