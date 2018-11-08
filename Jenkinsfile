properties([
    buildDiscarder(logRotator(numToKeepStr: '3'))
])
node('docker&&linux') {
    try {
        notifyBuild('STARTED')
        docker.withRegistry('https://registry.anderswind.dk', 'registry.anderswind.dk') {
            stage('Fetch SCM') {
                checkout scm
            }

            def large
            def initial
            stage('Website Build') {
                large = docker.build('resolved-landingpage:large', '-f resolved-website/Dockerfile resolved-website')
                initial = docker.build('resolved-landingpage:initial', '-f initial-page/Dockerfile initial-page')
            }

            stage('Push images') {
                large.push()
                initial.push()
            }
            currentBuild.result = "SUCCESS"
        }
    } catch (e) {
        // If there was an exception thrown, the build failed
        currentBuild.result = "FAILURE"
        throw e
    } finally {
        // Success or failure, always send notifications
        notifyBuild(currentBuild.result)
    }
}


def notifyBuild(String buildStatus = 'STARTED') {
    // Default values
    def colorCode
    def subject = "Build ${buildStatus}: Job '${env.JOB_NAME} [${env.BUILD_NUMBER}]'"
    def summary = "${subject}:\n(${env.BUILD_URL})"

    // Override default values based on build status
    if (buildStatus == 'STARTED') {
        colorCode = ''
    } else if (buildStatus == 'SUCCESS') {
        colorCode = 'good'
    } else if (buildStatus == 'UNSTABLE') {
        colorCode = 'warning'
    } else {
        colorCode = 'danger'
    }

    // Send notifications
    slackSend (color: colorCode, message: summary)
}