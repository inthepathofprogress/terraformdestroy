stage('Terraform Init') {
    steps {
        withCredentials([aws(credentialsId: "${env.AWS_CREDENTIALS_ID}", 
                           accessKeyVariable: 'AWS_ACCESS_KEY_ID', 
                           secretKeyVariable: 'AWS_SECRET_ACCESS_KEY')]) {
            sh 'terraform init -reconfigure'
        }
    }
}
