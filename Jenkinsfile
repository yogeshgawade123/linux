node
{
    stage('checkout')
    {
        checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/sagarlinux/hello-world-war.git']]])
    }
    stage('build'){
        sh 'mvn clean package'
    }
}
