@Library('lib') _
pipeline{
    agent any

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
