pipeline {
     agent any
     stages {
         stage('Build') {
             steps {
                 echo 'Building...'
             }
             post {
                 always {
                     jiraSendBuildInfo branch: 'MS-75-jenkins-branch', site: 'cfraga.atlassian.net'
                 }
             }
         }
         
     }
 }
