pipeline{
    agent any{
      stages{
        stage('Branch Based') {
          steps{
            script{
              def branch = env.BRANCH_NAME
              echo "branch we are in: ${branch}"
              if(branch == "main") {
                echo "main branch built"
              }
              else if (branch == "dev") {
                echo "Development branch built"
              }
              else eco "Running normally"
            }
          }
        }
      }
    }
}
