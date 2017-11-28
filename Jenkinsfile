stage('Build') {
  milestone()
  node {
    dir('Lab4' {
        sh './gradlew compileJava'
    }
  }
}

stage('Testing') {
  milestone()
  node {
      dir('Lab4' {
          sh './gradlew test'
      }
    }
}

stage('Deploy') {
  input "Deploy?"
  milestone()
  node {
    echo "Deploying"
  }
}