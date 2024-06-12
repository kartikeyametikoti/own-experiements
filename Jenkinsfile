pipeline{
    agent any
    stages{
        stage('getting git repo')
        {
            steps{
                git branch: 'main', credentialsId: 'my-credentials', url: 'https://github.com/kartikeyametikoti/own-experiements.git'
            }
        }
        stage('build and run')
        {
            steps{
                sh 'javac kartikeya.java'
                sh 'java kartikeya'
            }
        }
       
    }
}