node() {
    stage('Build') {
      milestone()
      checkout scm
            sh './gradlew compileJava'
    }

    stage('Testing') {
      milestone()
          dir('Lab4'){
              sh './gradlew test'
          }
    }

    stage('Deploy') {
      input "Deploy?"
      milestone()
        echo "Deploying"
    }
}