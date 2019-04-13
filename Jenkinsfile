node("docker") {

    stage("Checkout Project") {
        checkout scm
    }

    stage("Build Docker Image") {
            docker.build("docker.dragon.zone:10081/bitcoin-core:0.17.1.${env.BUILD_NUMBER}", "--build-arg revision=v0.17.1 .")
    }
}
