pipeline {
  agent any
  triggers { pollSCM('H/5 * * * *') }
  stages {
    stage('Build')                { steps { echo 'Building…' } }
    stage('Unit & Integration Tests') { steps { echo 'Testing…' } }
    stage('Code Analysis')        { steps { echo 'Analyzing code…' } }
    stage('Security Scan')        { steps { echo 'Scanning security…' } }
    stage('Deploy to Staging')    { steps { echo 'Deploying to staging…' } }
    stage('Integration Tests on Staging') { steps { echo 'Testing staging…' } }
    stage('Deploy to Production') { steps { echo 'Deploying to production…' } }
  }
}

