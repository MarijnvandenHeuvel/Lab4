stage('Build') {
  milestone()
  node {
    sh "./gradlew clean build"
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