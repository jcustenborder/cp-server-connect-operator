#!groovy
@Library('jenkins-pipeline') import com.github.jcustenborder.jenkins.pipeline.ConnectDockerPipeline

def pipe = new ConnectDockerPipeline()
pipe.imageName = 'cp-server-connect-operator'
pipe.majorVersion = 5
pipe.minorVersion = 5
pipe.patchVersion = 1
pipe.repositories = [
    ['credential': 'hub.docker.com', 'registry': 'https://registry.hub.docker.com', 'repository': 'jcustenborder']
]
pipe.execute()

