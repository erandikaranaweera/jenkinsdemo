node {

    checkout scm
    tools {dockerTool  "docker" }
    docker.withRegistry('https://registry.hub.docker.com', 'docker-hub') {

        def customimage = docker.build("erandiranaweera/cw")

        /* Push the container to the custom Registry */
        customimage.push()
    }
}
