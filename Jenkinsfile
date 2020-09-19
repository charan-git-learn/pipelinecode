node {
   stage('Git clone'){
       git credentialsId: 'bbf5cb79-1294-4fd9-ac8a-b36f6d205ad8', url: 'https://github.com/charan-git-learn/apple-project.git'
    }
   stage('clean') {
         sh "mvn clean"
    }    
    stage('compile') {
         sh "mvn compile" 
    }
    stage('package') {
         sh "mvn package"
    }
    stage('deploy') {
         sh "mvn deploy"
    }
}  
