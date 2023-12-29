pipeline {
    agent any

    stages {
           stage('Fetch code') {
                   steps {
                         git branch: 'main', url: 'https://github.com/Dhruvakumarkr/html.git'
                         }
                }

           stage('Installing Apache') {
                   steps {
                         sh 'sudo apt install apache2'
                         }
                }

           stage('Deploying Application') {
                   steps {
                         sh 'sudo cp -R * /var/www/html/'
                         }
                }

           }
}
