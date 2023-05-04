pipeline {
    agent any

    stages {
        stage('Code Quality') {
            steps {
                echo 'Code Quality'
                sh 'env'
            }
        }
        stage('Style Checks') {
            when {
                branch 'main'
            }
            steps {
                echo 'Style Checks'
            }
        }
        stage('Unit Tests') {
            when {
                branch 'main'
            }

            steps {
                echo 'Unit Tests'
            }
        }
        stage('Download Dependancies') {
            when { tag "*" }
            steps {

                echo 'Download Dependancies'
            }
        }
        stage('Prepare Artifacts') {
            when { tag "*" }
            steps {
                echo 'Prepare Artifacts'
            }
        }

        stage('Publish Artifacts') {
            when { tag "*" }
            steps {
                echo 'Publish Artifacts'
            }
        }

    }


}