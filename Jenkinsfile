stage('Build') {
  milestone()
  node {
    gradlew clean build
  }
}

stage('Testing') {
  milestone()
  node {
    gradlew test
  }
}

stage('Deploy') {
  input "Deploy?"
  milestone()
  node {
    echo "Deploying"
  }
}