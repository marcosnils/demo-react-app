pipeline {
  agent { label 'dagger' }
  
  environment {
    _EXPERIMENTAL_DAGGER_CLOUD_TOKEN = "a276ce43-e1ca-4427-a6ee-200d77b85b56"
  }
  stages {
    stage("dagger") {
      steps {
        sh '''
            npm i @dagger.io/dagger@0.8.4
            dagger run npm run ci
        '''
      }
    }
  }
}