pipeline 
{
    agent any
    stages 
{         
    stage('checkout')
    {
    steps
    {
    checkout changelog: false, poll: false, scm: [$class: 'GitSCM', 
branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: 
false, extensions: [], submoduleCfg: [], userRemoteConfigs: 
[[credentialsId: 'git-creds', url: 
'https://github.com/deepakirthi/my-app.git']]]
    }
    } 
    stage('git credentials')
    { 
    steps
    {
      git changelog: false, credentialsId: 'git-creds', poll: false, 
url: 'https://github.com/deepakirthi/my-app.git'
    }
    }
}
}





























