node {



stage ('scm-checkout') {
 

checkout([$class: 'GitSCM',
 branches: [[name: '*/master']], 
 doGenerateSubmoduleConfigurations: false, 
 extensions: [], submoduleCfg: [], 
 userRemoteConfigs: [[url: 'https://github.com/NilimaHVaidya/NewRepoDemo.git']]])

}



 stage ('build') {

sh 'mvn -f pom.xml clean package'


}

}