#!groovy
@Library('jenkins-pipeline') import com.github.jcustenborder.jenkins.pipeline.ConnectDockerPipeline

def pipe = new ConnectDockerPipeline()
pipe.imageName = 'cp-server-connect-operator'
pipe.majorVersion = 6
pipe.minorVersion = 1
pipe.patchVersion = 1
pipe.repositories = [
    ['credential': 'custenborder_docker', 'registry': 'https://docker.custenborder.com', 'repository': 'jcustenborder']
]
pipe.execute()

