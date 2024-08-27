pipeline {
    agent any
    environment {
        GIT_SSL_NO_VERIFY = 1
    }
    stages {
        stage('gitlab-clone') {
            steps {
                git branch: 'master', credentialsId: 'gitlab', url: 'https://gitlab.115.68.198.99.nip.io/root/task_msa_ui.git'
            }
        }
    }
}