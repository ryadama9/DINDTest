node("jenkins-mahwahtech-test") {
  git branch: 'main', url: 'https://github.com/ryadama9/DINDTest.git'
        stage("Build"){
            container(name: 'buildah'){
                script {
                    //sleep 99999
                    sh "buildah build -t buildah-test:1 ."
                    //sh "/kaniko/executor --dockerfile Dockerfile --context `pwd` --destination quay.io/volvocars/test-kaniko:latest"
                    }
                }
        }
}
