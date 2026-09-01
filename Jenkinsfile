pipeline {
    agent any

    triggers {
        pollSCM('H/1 * * * *')
    }

    stages {

        stage('Build') {
            steps {
                echo 'Build the code using Maven as the build automation tool to compile and package the application. We made an update here!'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Run unit tests using JUnit and integration tests using Selenium.'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Analyse the code using SonarQube to identify code quality issues and potential vulnerabilities.'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Perform a security scan using OWASP Dependency-Check to identify known vulnerabilities.'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Deploy the application to a staging server using AWS EC2.'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Run integration tests on the staging environment using Selenium to verify the application.'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Deploy the application to the production server using AWS EC2.'
            }
        }
    }
}
