node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'abdel-cred') {

        def customImage = docker.build("abdelouahed79/nodjs.app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
