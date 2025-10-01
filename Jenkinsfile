pipeline {
    agent any
    stages {
        stage('Stage 0') {
    steps {
        withEnv(["MY_ENV=VALUE"]) {
            registerBuildArtifactMetadata(
                name: "e2e-artifact-stage-PROD-test-001",
                version: "0.0.2",
                type: "docker",
                url: "http://your-url-here.com",
                digest: "6u637064707039346163663930",
                label: "prod-e2e"
            )
        }
    }
    }
    }
}