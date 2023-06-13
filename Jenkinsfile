node("jenkins-mahwahtech-test") {
        stage("Build"){
            container(name: 'build'){
                script {
                    //sleep 99999
                    sh "buildah build-using-dockerfile -t buildah-test:${currentBuild.number} ."
                    sleep 9999
                    //sh "/kaniko/executor --dockerfile Dockerfile --context `pwd` --destination quay.io/volvocars/test-kaniko:latest"
                    }
                }
        }
}
