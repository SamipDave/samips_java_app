pipeline {
    agent any

    stages {
        stage('gitcheckout') {
            steps {
                git branch: 'main', url: 'https://github.com/SamipDave/samips_java_app.git'
            }
        }
    }
}
