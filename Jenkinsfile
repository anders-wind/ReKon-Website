properties([
    buildDiscarder(logRotator(numToKeepStr: '3'))
])
node('docker&&linux') {
    stage('Fetch SCM') {
        checkout scm
    }
    def large
    def initial
    stage('Website Build') {
        large = docker.build('registry.anderswind.dk/resolved-landingpage:large', '-f resolved-website/Dockerfile resolved-website')
        initial = docker.build('registry.anderswind.dk/resolved-landingpage:initial', '-f initial-page/Dockerfile initial-page')
    }
    stage('Push images') {
        large.push()
        initial.push()
    }
}