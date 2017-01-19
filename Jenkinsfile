node {
   stage('Preparation') {
      git 'https://github.com/vikramv911/HerokuJenkinsLab.git'
   }
   stage('Build') {
      sh "./gradlew clean test"
   }

   stage('Deploy'){
    sh "git push https://git.heroku.com/morning-reef-60105.git master"
   }
}