pipeline {
  agent any 

  stages {
    stage('Clone Repository'){
      steps {
        git url: 'https://github.com/omkarsathe01/jenkin-practice', branch: 'main'
      }
    }

    stage('Create Containers'){
      steps {
        sh '''
        echo "Current Directory:"
        pwd
        echo "Listing files:"
        ls -ltra
        docker compose up
        '''
      }
    }
  }
}
