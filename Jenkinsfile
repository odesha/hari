node
{
    stage "1. install docker"
    sh "yum install docker -y"
    
    stage "2. Start the service"
    sh "service docker start"
    
    stage "3. Build the image"
    sh "docker build -t jenkinsfile_image_har /home/ec2-user"
    
    stage "4. Run the container"
    sh "docker run -dit --name jenkinsfile_container_har jenkinsfile_image_har"
    
    stage "5. Push the image"
    sh "docker login --username odesha --password Welcome@9"
    
    sh "docker tag jenkinsfile_image_har odesha/jenkinsfile_image_har"
    
    sh "docker push odesha/jenkinsfile_image_har"
}
