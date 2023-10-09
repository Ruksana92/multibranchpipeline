pipeline {
    agent any
    stages {
        stage('Main Branch Deploy Code') {
            when {
                branch 'main'
            }
            steps {
                sh """
                echo "Building Artifact from Main branch"
                """

                sh """
                echo "Deploying Code from Main branch"
                """
            }
        }
        stage('Developer Branch Deploy Code') {
            when {
                branch 'developer'
            }
            steps {
                sh """
                echo "Building Artifact from Developer branch"
                """
                sh """
                echo "Deploying Code from Developer branch"
                """
           }
        }
    }
}
