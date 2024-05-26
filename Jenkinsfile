pipeline { 
   agent any

   stages {

    stage('Clone Repository') {
      steps { 
        git 'https://github.com/SAROSURYA/testangular.git -b main'
      } 
    }

    stage('Build and Run with Docker Compose') {
      steps {
        script {
          sh 'docker-compose up -d'
        }
      }
    }
    
   }
}
