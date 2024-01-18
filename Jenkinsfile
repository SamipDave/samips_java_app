@Library('lib') _
pipeline {
    agent any

    stages {
        stage('gitcheckout') {
            steps {
                    url: "https://github.com/SamipDave/samips_java_app.git"
                    branch: "main"
                }
            }
        }
        stage('unit Test mvn') {
            steps {
                    mvnTest()
        }
    }
}
