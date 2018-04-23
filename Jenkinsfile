node {
    stage('Initialize'){
        def server = Artifactory.newServer url: 'https://spdmaven2.fnis.com/artifactory/fis-repos', credentialsId: 'artifactory-user'
        def uploadSpec = """{
            "files": [
                {
                  "pattern": "jenkins-pipeline-examples/resources/.*A[A-z]tifactory.*.zip",
                  "target": "libs-snapshot-local/",
                  "regexp": "true"
                },
                {
                  "pattern": "jenkins-pipeline-examples/resources/.*(A|a)rtifactory.*.zip",
                  "target": "libs-snapshot-local/",
                 "regexp": "true"
                }
            ]
        }"""
        server.download(downloadSpec)
    }
    
    
}
