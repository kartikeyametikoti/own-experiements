pipeline{
    agent any
    stages{
        stage('getting git repo')
        {
            steps{
                git branch: 'main', credentialsId: 'my-credentials', url: 'https://github.com/kartikeya-1112/projectdemo'
            }
        }
        stage('build and run')
        {
            steps{
                sh 'javac kartikeya.java'&& 'java kartikeya'
            }
        }
       
    }
}