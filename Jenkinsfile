pipeline {
    agent any
    environment {
        GIT_SSL_NO_VERIFY = true
    }
    stages {
        stage('Pre-Checkout') {
            steps {
                sh "git config http.sslVerify false"
            }
        }
        stage('Scm Checkout') {
            steps {
                git branch: 'master', credentialsId: 'glpat-55AexEZPJxR5a7sS2DkX', url: 'https://gitlab.115.68.198.99.nip.io/root/task_msa_ui.git'
            }
        }
    }
}
