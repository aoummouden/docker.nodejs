node {
    checkout scm

    docker.withRegistry('https://registry.example.com', 'abdel-cred') {

        def customImage = docker.build("abdelouahed79:${env.BUILD_ID}")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
