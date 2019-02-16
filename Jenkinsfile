def workspace;

node
{
    stage('Checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/tirumalamoger/My-pipeline-jenkinsfile.git']]])
        workspace = pwd()
    }
    
    stage('CodeAnalysis')
    {
        echo 'Analysing the code'
    }
    
    stage('Build')
    {
        echo 'Build the implemented code'
    }
    
    stage('UnitTesting')
    {
        echo 'Perform the Unit testing'
    }
    
    stage('Delivery')
    {
        echo "Push the code to application"
    }
}
