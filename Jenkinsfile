pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code...'

                git branch: 'b1',
                url: 'https://github.com/Tanishqkathed/for_jenkins_test.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Running Build Stage...'

                sh '''
                mkdir -p build
                echo "Build completed successfully" > build/build.txt
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Running Test Stage...'

                sh '''
                echo "Executing tests..."
                echo "All tests passed"
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Running Deploy Stage...'

                sh '''
                echo "Deploying application..."
                echo "Deployment successful"
                '''
            }
        }
    }
}pipeline {
    agent any

    triggers {
        pollSCM('H/2 * * * *')
    }

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code...'

                git branch: 'b1',
                url: 'https://github.com/Tanishqkathed/for_jenkins_test.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Running Build Stage...'

                sh '''
                mkdir -p build
                echo "Build completed successfully" > build/build.txt
                '''
            }
        }

        stage('Test') {
            steps {
                echo 'Running Test Stage...'

                sh '''
                echo "Executing tests..."
                echo "All tests passed"
                '''
            }
        }

        stage('Deploy') {
            steps {
                echo 'Running Deploy Stage...'

                sh '''
                echo "Deploying application..."
                echo "Deployment successful"
                '''
            }
        }
    }
}
