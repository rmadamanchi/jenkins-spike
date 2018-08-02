#!groovy

echo "Running ${env.BRANCH_NAME}"

if (env.BRANCH_NAME != 'master') {
    stage('Sleep') {
        echo "Sleeping"
        if (currentBuild.changeSets != null) {
          for (changeSetList in currentBuild.changeSets) {
              for (changeSet in changeSetList) {
                 echo changeSet.msg
                 echo changeSet.id
              }
          }
        }
        sleep 30
    }
}
