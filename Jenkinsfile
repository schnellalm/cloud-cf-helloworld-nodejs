@Library('piper-lib-os') _
agent {
        docker { image '510e9ffc2cfd' }
    }
    stage('prepare') {
        checkout scm
        setupCommonPipelineEnvironment script:this
    }
stage('build') {
    mtaBuild script: this
}
