CODE_CHANGES = getGitChanges()
pipeline{
  agent any 
  stages{
    stage("build"){
      steps{
        echo 'building the application.....'
        }
      }
    stage("test"){
      when{
        expresson{
          BRANCH_NAME = 'development'
        }
      }
      steps{
        echo 'testing the application.....'
      }
    }
    stage("deploy"){
      steps{
        echo 'deploying the application.....'
      }
    }
  }
}
