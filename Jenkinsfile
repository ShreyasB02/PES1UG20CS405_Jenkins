pipeline{
  agent any
  
  stages{
    stage('Build') {
      steps {
        sh 'g++ -c PES1UG20CS405.cpp - error'
        sh 'g++ -o PES1UG20CS405 PES1UG20CS405.cpp'
        echo 'Build Succesful'
      }
    }
    stage('Test') {
      steps {
           sh  './PES1UG20CS405'
           echo 'Test Was Succesful'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy Succesful'
      }
    }
  }
  post{
    failure{
      echo 'Pipeline Failed'
    }
  }
}
