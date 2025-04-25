pipeline{
  agent any
  
  stages{
    stage('web app') {
      steps{
        sh ' sudo apt install nginx -y'
      }
    }
    stage('default page removal') {
      steps{
        sh 'sudo rm -rf var/www/html/*'
      }
    }
  }
}
  
