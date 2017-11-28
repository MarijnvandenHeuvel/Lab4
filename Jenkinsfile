stage('Build') {
  milestone()
  node {
    def gradleHome = tool 'gradle
    bat(/"${gradleHome}\bin\gradle" clean build/)
  }
}

stage('Testing') {
  milestone()
  node {
    def gradleHome = tool 'gradle'
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