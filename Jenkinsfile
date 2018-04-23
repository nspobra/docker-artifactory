pipeline {
    agent none
    def server = Artifactory.newServer url: 'https://spdmaven2.fnis.com/artifactory/fis-repos', credentialsId: 'artifactory-user'
    stages {
        stage('Checkout') {
            checkout scm
        }
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
