node("docker") {

    stage("Checkout Project") {
        checkout scm
    }

    stage("Build Docker Image") {
            docker.build("docker.dragon.zone:10081/bitcoin-core:0.15.0.1.${env.BUILD_NUMBER}", "--build-arg revision=v0.15.0.1 .")
    }
}
