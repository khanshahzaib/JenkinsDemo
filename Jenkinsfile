pipeline { 
        agent any

    stages {
        stage('Clone/ Fetch from Git') {
            steps {
                git branch: 'main', url: 'https://github.com/khanshahzaib/JenkinsDemo'
                echo 'succesfully git connection made'
            }
        }
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying'
                bat "mvn clean"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        stage('Release') {
            steps {
                echo 'Releasing'
            }
        }
    }
}
