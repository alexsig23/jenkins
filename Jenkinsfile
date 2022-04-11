pipeline {
    agent any
    parameters {
        string(name: 'colo', defaultValue: 'red', description: 'fave color?')
    }
    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                 echo "${params.colo} is my favourite colorrr!"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying - gotta figure out how to have docker/vagrant pod with some app for deploying'
            }
        }
    }
}
