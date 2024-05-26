pipeline { 
   agent any

   stages {

    stage('Clone Repository') {
      steps { 
        git branch: "main", url: 'https://github.com/SAROSURYA/testangular.git'
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
