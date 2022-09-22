node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub'){
        def customImage = docker.build("oryzasativa29/godocker")
        customImage.push()
    }
    
    # deploy to kubernetes
   # kubernetesDeploy(configs: "deploymentservice.yml", kubeconfigId: "kubernetes")
}
