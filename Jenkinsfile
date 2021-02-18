node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerIdentity') {
        
        def customImage = docker.build("kirtigupta123/add")
        

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
