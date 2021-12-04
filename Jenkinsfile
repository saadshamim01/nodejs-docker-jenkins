node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {
    
        def customImage = docker.build("saadshamim01/nodejs-app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}