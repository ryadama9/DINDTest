node("jenkins-mahwahtech-test") {
        stage("Build"){
            container(name: 'build'){
                steps {
                    git branch: 'main',
                        url: 'git@https://github.com/ryadama9/DINDTest.git'
                    sleep 99999
                    sh "buildah build -t buildah-test:1 ."
                    sleep 9999
                    //sh "/kaniko/executor --dockerfile Dockerfile --context `pwd` --destination quay.io/volvocars/test-kaniko:latest"
                    }
                }
        }
}
