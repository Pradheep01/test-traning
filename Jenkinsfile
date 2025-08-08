pipeline {
    agent any //any indictaes any env
  
  
    triggers(
//build is trriggred when push event is recived from github webhook 
      githubPush()
    )


stages(

stage('Checkout'){
  steps {
                git branch: 'main', url: 'https://github.com/Pradheep01/test-traning.git'
            }
}
  stage('Build'){
  steps {
              echo 'Runing the build'
            }
}

  stage('Test'){
  steps {
                echo 'Runung Test'
            }
}

  stage('Deploy'){
  steps {
                echo 'Deploy the build'
            }
}

)

post{
  success{
    echo 'Script has passed'
  }
  failure {
    echo 'Build has failed'
  }
}
}
