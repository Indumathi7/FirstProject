pipeline{
  agent any 

  stages{
    stage('Checkout'){
      steps{
      checkout scm
      }
    }

    stage('Build'){
      steps{
      sh 'javac Sample.java'
      }
    }

    stage('Run'){
      steps{
        sh 'java Sample'
      }
    }
  }

  post{
    success{
      echo 'executed sucessfully'
    }
    failure{
      echo 'job failed'
    }
  }
}
  
