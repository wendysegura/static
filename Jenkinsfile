pipeline {
  agent any
  stages {
    stage('Lint HTML') {
      steps {
        sh 'tidy -q -e *.html'
      }
    }
    stage('Upload to AWS') {
      steps {
        withAWS(region:'us-west-1', credentials: 'aws-static') {
          s3Upload(file:'index.html', bucket:'jenkinsudacity', path:'https://jenkinsudacity.s3.amazonaws.com/index.html')
        }
      }
    }
  }
}
