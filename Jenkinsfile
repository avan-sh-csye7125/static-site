node {
    checkout scm

    def customImage = docker.build("static-site:${env.BUILD_ID}")
    customImage.inside {
        sh 'echo "Hello World"'
    }
}

    docker.withRegistry('https://registry.example.com', 'credentials-id') {
        def customImage = docker.build("avaneeshy/static-site:${env.BUILD_ID}")
        /* Push the container to the custom Registry */
        customImage.push()
    }

