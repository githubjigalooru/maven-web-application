properties([[$class: 'JiraProjectProperty'], buildDiscarder(logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '', daysToKeepStr: '5', numToKeepStr: '5')), parameters([choice(choices: ['master', 'stage', 'uat', 'prepro'], description: 'single job implimenting the declarative pipeline', name: 'Branch')]), [$class: 'JobLocalConfiguration', changeReasonComment: ''], pipelineTriggers([pollSCM('* * * * *')])])

pipeline{
    agent any
    stages {
        stage("scm_checkout") {
            steps {
              sh "echo first step completed"    
                
            }
