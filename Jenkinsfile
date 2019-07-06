pipeline {
  agent any
  stages {
    stage('Git Checkout') {
      steps {
        git(url: 'https://github.com/Nadeemalvi/DevOpsClassCodes.git', branch: 'master', poll: true)
      }
    }
    stage('Compile') {
      steps {
        build 'Addressbook_Compile'
      }
    }
    stage('Code Review') {
      steps {
        build 'Addressbook_CodeReview'
      }
    }
  }
}