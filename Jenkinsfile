stage('Build') {
  milestone()
  node {
    build
  }
}

stage('Testing') {
  milestone()
  node {
    test
  }
}

stage('Deploy') {
  input "Deploy?"
  milestone()
  node {
    echo "Deploying"
  }
}