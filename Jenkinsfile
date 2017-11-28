stage('Build') {
  milestone()
  node {
    sh('./gradlew compileJava')
  }
}

stage('Testing') {
  milestone()
  node {
     sh './gradlew test'
  }
}

stage('Deploy') {
  input "Deploy?"
  milestone()
  node {
    echo "Deploying"
  }
}