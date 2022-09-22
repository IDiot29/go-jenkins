pipeline {
    checkout scm
    docker.withRegistry('https://hub.docker.com', 'dockerhub'){
        def customImage = docker.build("oryzasativa29/godocker")
        customImage.push()
    }
}
