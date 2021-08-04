#!groovy
@Library('jenkins-pipeline') import com.github.jcustenborder.jenkins.pipeline.ConnectDockerPipeline

def pipe = new ConnectDockerPipeline()
pipe.imageName = 'cp-server-connect-operator'
pipe.majorVersion = 6
pipe.minorVersion = 0
pipe.patchVersion = 0
pipe.repositories = [
    ['credential': 'hub.docker.com', 'registry': 'https://registry.hub.docker.com', 'repository': 'jcustenborder']
]
pipe.execute()

