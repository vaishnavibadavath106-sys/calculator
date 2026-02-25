pipeline{
  agent any
  stages{
    stage('clone')
    steps{
      git branch:'main',url:'https://github.com/vaishnavibadavath106-sys/calculator.git';
    }
  }
  stage('compile'){
    steps{
      sh 'java calculator.java'
    }
  }
  stage('build'){
    steps{
      sh 'java calculator 25 5'
    }
  }
   stage('test'){
    steps{
      sh 'java calculator 30 -5'
    }
   }
   stage('deploy'){
    steps{
      echo 'deployment completed'
    }
   }
}


