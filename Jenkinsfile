#!groovy

echo "Running ${env.BRANCH_NAME}"

if (env.BRANCH_NAME != 'master') {
    stage('Sleep') {
        echo "Sleeping"
        echo "ChangeSets"
        echo currentBuild.changeSets
        if (currentBuild.changeSets != null) {
          for (changeSetList in currentBuild.changeSets) {
              echo "ChangeSetList"
              echo changeSetList
              for (changeSet in changeSetList) {
                  echo "ChangeSet"
                  echo changeSet
                 echo changeSet.msg
                 echo changeSet.id
              }
          }
        }
        sleep 30
    }
}
