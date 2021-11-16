pipeline{
agent any
tools{
maven 'maven'
jdk 'Jdk-8'
}
stages{
stage('git' ){
steps{
git credentialsId:'github',url:'https://github.com/saba989.git'
}
}
stage('build'){
steps{
bat 'mvn -f  library/libraryclient/pom.xml clean install'
}
}
}
}
