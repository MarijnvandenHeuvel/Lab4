node() {
    stage('Build') {
        milestone()
        checkout scm
        sh './gradlew compileJava'
    }

    stage('Testing') {
        milestone()
        sh './gradlew test'
    }
}