node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub-credentials') {

        def customImage = docker.build("sudhakshara/nodeapp")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
