node {
    stage('Build') {
      milestone()
      sh './gradlew compileJava'
    }

    stage('Testing') {
      milestone()
      sh './gradlew test'
    }

    stage('Deploy') {
      input "Deploy?"
      milestone()
      echo "Deploying"
    }
}