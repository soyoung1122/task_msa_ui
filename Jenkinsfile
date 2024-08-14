pipeline {
    agent any
    stages {
        stage('github-clone') {
            steps {
                git branch: 'master', credentialsId: 'dbe5b517-180b-4db4-99ce-fd94d03160a4', url: 'https://github.com/soyoung1122/task_msa_ui.git'
            }
        }
    }
}