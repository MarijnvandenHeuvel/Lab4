node {
    stage('Build') {
      milestone()
      dir ('Lab4') {
      sh './gradlew compileJava'
    }
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