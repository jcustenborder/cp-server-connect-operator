#!groovy
@Library('jenkins-pipeline') import com.github.jcustenborder.jenkins.pipeline.ConnectDockerPipeline

def pipe = new ConnectDockerPipeline()
pipe.imageName = 'cp-server-connect-operator'
pipe.majorVersion = 5
pipe.minorVersion = 5
pipe.patchVersion = 2
pipe.repositories = [
    ['credential': 'custenborder_docker', 'registry': 'https://docker.custenborder.com', 'repository': 'jcustenborder']
]
pipe.execute()

