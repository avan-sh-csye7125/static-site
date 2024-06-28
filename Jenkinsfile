node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub-credentials') {
        def customImage = docker.build("avaneeshy/static-site:main")
        
        if (env.BRANCH_NAME == 'main') {
            customImage.push()
        }

    }
        
}

