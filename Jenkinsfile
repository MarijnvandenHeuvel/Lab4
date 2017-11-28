stage('Build') {
  milestone()
  node {
    echo "Building"
  }
}

stage('Testing') {
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