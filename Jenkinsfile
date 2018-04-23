node {
    stage('Initialize'){
        def server = Artifactory.newServer url: 'https://spdmaven2.fnis.com/artifactory/fis-repos', credentialsId: 'artifactory-user'
        def downloadSpec = """{
         "files": [
          {
              "pattern": "bazinga-repo/*.zip",
              "target": "bazinga/"
            }
         ]
        }"""
        server.download(downloadSpec)
    }
    
    
}
