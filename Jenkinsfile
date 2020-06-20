@Library('piper-lib-os') _
pipeline {
    agent {
        docker { image '510e9ffc2cfd' }
    }
    stages {
        stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
    stage('build') {
    mtaBuild script: this
    }
   }
}
            
            
