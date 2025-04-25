pipeline{
  agent any
  
  stages{
    stage('web app') {
      steps{
        sh ' sudo apt install nginx -y'
      }
    }
    stage ('default page removel') {
      steps{
        sh 'sudo rm -rf /var/www/html/*'
      }
    }
    stage ('deployment') {
      steps{
        sh 'sudo cp -rf  /home/azureuser/workspace/eccom/* /var/www/html/'
      }
    }
    stage ('restart') {
      steps{
        sh 'sudo systemctl restart nginx'
      }
    }

  }
}
  
