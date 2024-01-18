@Library('lib') _
pipeline {
    agent any

    stages {
        stage('gitcheckout') {
            steps {
                script{
                    url: "https://github.com/SamipDave/samips_java_app.git"
                }
            }
        }
        stage('unit Test mvn') {
            steps {
                script{
                    mvnTest()  
            }
        }
    }
}
}
