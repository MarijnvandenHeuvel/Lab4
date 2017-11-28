stage('Build') {
  milestone()
  node {
    echo "Building"
  }
}

stage('Test') {
  milestone()
  node {
    echo "Testing"
  }
}

stage('Deploy') {
  input "Deploy?"
  milestone()
  node {
    echo "Deploying"
  }
}