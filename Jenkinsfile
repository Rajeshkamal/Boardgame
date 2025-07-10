pipeline {
    agent any

    tools {
        maven 'mavne3.6'
        jdk 'jdk17'
    }
    stage {

        stage('Compile') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('test') {
            steps {
                sh 'mvn test '
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
