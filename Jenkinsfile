pipeline {
    agent any

    triggers {
        githubPush()
    }

    stages {
        stage('Clone Repository') {
            steps {
                git branch: 'main' url: 'https://github.com/ruchiradevane/Java-Jenkins-Demo.git'
            }
        }

        stage('Compile Java') {
            steps {
                bat 'javac HelloWorld.java'
            }
        }

        stage('Run Java Program') {
            steps {
                bat 'java HelloWorld'
            }
        }
    }
}
