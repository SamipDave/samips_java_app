@Library('lib') _
pipeline{
    agent any
    
   tools{
        jdk 'jdk17'
        maven 'maven3'
    }
    stages {
        stage('gitCheckout') {
            steps {
            gitCheckout(
                branch: "main",
                url: "https://github.com/SamipDave/samips_java_app.git"
                        )
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
}
