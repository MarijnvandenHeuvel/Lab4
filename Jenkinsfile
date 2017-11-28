def gradleHome = tool 'gradle'

stage('Build') {
  milestone()
  node {
    bat(/"${gradleHome}\bin\gradle" clean build/)
  }
}

stage('Testing') {
  milestone()
  node {
    bat(/"${gradleHome}\bin\gradle" clean test/)
  }
}

stage('Deploy') {
  input "Deploy?"
  milestone()
  node {
    echo "Deploying"
  }
}