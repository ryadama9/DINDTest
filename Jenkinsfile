node("jenkins-mahwahtech-test") {
    git branch: 'main', url: 'https://github.com/ryadama9/KanikoTest.git'
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
