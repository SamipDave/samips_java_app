@Library('lib') _
pipeline{
    agent any
    tools { maven 'maven3.8.1'
    }

    stages {
        stage('gitCheckout') {
            steps {
                script{
                    gitCheckout(
                        branch: "main",
                        url: "https://github.com/SamipDave/samips_java_app.git"
                        )
            }
        }
    }
        stage('mvnTest') {
            steps {
                script{
                    mvnTest()
            }
        }
    }
}
}
