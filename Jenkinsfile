def server = Artifactory.newServer url: 'https://spdmaven2.fnis.com/artifactory/fis-repos', credentialsId: 'artifactory-user'
pipeline {
    agent none
    stages {
        stage('Example') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
