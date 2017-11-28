node() {
    stage('Build') {
        milestone()
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: '303bf04f-4bc2-4057-9662-a8c05f311735', url: 'https://github.com/MarijnvandenHeuvel/Lab4.git']]])
        sh 'chmod +x ./gradlew'
        sh './gradlew compileJava'
    }

    stage('Testing') {
        milestone()
        sh './gradlew clean test'
        junit 'build/test-results/**/*.xml'
    }
}