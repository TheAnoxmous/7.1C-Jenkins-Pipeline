pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1 - Build: Compile the source code and package it into a deployable artefact'
                echo 'Tool: Maven'
            }
        }
        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2 - Unit and Integration Tests: Unit tests verify individual functions; integration tests verify components work together'
                echo 'Tools: JUnit (unit tests), Selenium (integration tests)'
            }
        }
        stage('Code Analysis') {
            steps {
                echo 'Stage 3 - Code Analysis: Check code quality, complexity and adherence to industry coding standards'
                echo 'Tool: SonarQube'
            }
        }
        stage('Security Scan') {
            steps {
                echo 'Stage 4 - Security Scan: Scan the code and its dependencies for known vulnerabilities (CVEs)'
                echo 'Tool: OWASP Dependency-Check'
            }
        }
        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5 - Deploy to Staging: Deploy the packaged application to a staging server (AWS EC2 instance)'
                echo 'Tool: Ansible'
            }
        }
        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6 - Integration Tests on Staging: Run integration tests in a production-like environment'
                echo 'Tool: Selenium'
            }
        }
        stage('Deploy to Production') {
            steps {
                echo 'Stage 7 - Deploy to Production: Deploy the application to the production server (AWS EC2 instance)'
                echo 'Tool: Ansible'
            }
        }
    }
}
