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
                script{
                    gitCheckout(
                        branch: "main",
                        url: "https://github.com/SamipDave/samips_java_app.git"
                        )
                    }
                }
        }
        stage('unit test maven') {
            steps {
                script{
                        mvnTest()
                    }
                }
            }
        }
    
}
