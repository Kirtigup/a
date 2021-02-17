node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'DockerIdentity') {
        bat '@FOR /f "tokens=*" %i IN ('docker-machine.exe env') DO @%i'
        def customImage = docker.build("kirtigupta123/add")
        

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
