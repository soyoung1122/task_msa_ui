pipeline {
    agent any
    environment {
        GIT_SSL_NO_VERIFY = true
    }
    stages {
        stage('Git Config Setting') {
            steps {
                sh 'git config --global http.sslVerify false'
            }
        }
        stage('Git Clone') {
            steps {
                git branch: 'master', credentialsId: 'glpat-55AexEZPJxR5a7sS2DkX', url: 'https://gitlab.115.68.198.99.nip.io/root/task_msa_ui.git'
            }
        }
    }
}
