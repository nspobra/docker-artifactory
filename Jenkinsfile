node {
    stage('Initialize'){
        def server = Artifactory.newServer url: 'https://spdmaven2.fnis.com/artifactory/fis-repos', credentialsId: 'artifactory-user'
        def downloadSpec = """{
         "files": [
          {
              "pattern": "com/fisglobal/WebClient/7.6.2.3/*.jar",
              "target": "WebClient/"
            }
         ]
        }"""
        server.download(downloadSpec)
    }
    
    
}
