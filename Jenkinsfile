pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                echo 'Info of GitHub Repo'
                git 'https://github.com/JebaKishore18/my-first-repo.git'
            }
        }
        stage('Publish') {
            steps {
                  publishHTML([allowMissing:true, alwaysLinkToLastBuild:false, keepAll:false , reportDir:'.' , reportFiles: 'Love.html' , reportName:'HtmlReport'])
            }
        }
    }
}
