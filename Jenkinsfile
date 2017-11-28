
    stage('Build') {
      milestone()
      node {
       bat(/"gradlew\bin\gradle" clean build/)
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