pipeline {
   agent any

   stages {
       stage('Checkout')
       {
           steps {
               echo 'Checking out..'
               sh 'java -version'
               checkout([$class: 'GitSCM', branches: [[name: 'feature/chakra']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'GIT_Credentials', url: 'https://github.com/devopsmonks/hello-world-java.git']]])
           }
       }
}

