pipeline {
    agent any
    environment {
        GIT_SSL_NO_VERIFY = 'true;
    }
    stages {
        stage('Disable SSL Verification') {
            steps {
                sh 'git config --global http.sslVerify false'
            }
        }
        stage('gitlab-clone') {
            steps {
                git branch: 'master', credentialsId: 'gitlab', url: 'https://gitlab.115.68.198.99.nip.io/root/task_msa_ui.git'
            }
        }
    }
}
