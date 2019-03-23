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
    
        stage('Code Review')
          {
            steps {
                sh 'mvn -P metrics pmd:pmd'
                  }
           }
        
    stage('Testing')
          {
            steps {
                sh 'mvn test'
                  }
           }
        stage('Deploying')
          {
            steps {
                sh 'mvn deploy'
                  }
           }
}
}
