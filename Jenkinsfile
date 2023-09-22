pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        bat 'cacls run_build_script.sh /E /G Users:R'
        bat 'takeown /F run_build_script.sh'
      }
    }
    stage('Test') {
      steps {
       echo "Run tests" 
      }
    }
  }
}
