pipeline{
  agent:any
  stages{
    stage("checkout code"){
      steps{
        git branch: "main",
          url: 'https://github.com/Dhruvpatel272/jenkins-demo-app.git'
      }
}
    stages('Run script'){
      steps{
        sh 'chmod +x app.sh'
        sh'./app.sh'
      }
    }
  }
}
