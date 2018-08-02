#!groovy

echo "Running ${env.BRANCH_NAME}"

if (env.BRANCH_NAME != 'master') {
    stage('Sleep') {
        echo "Sleeping"
        echo "ChangeSets"
        echo currentBuild.changeSets.dump()
        if (currentBuild.changeSets != null) {
          for (changeSetList in currentBuild.changeSets) {
              echo "ChangeSetList"
              echo changeSetList.dump()
              for (changeSet in changeSetList) {
                  echo "ChangeSet"
                  echo changeSet.dump()
                 echo changeSet.msg
                 echo changeSet.id
              }
          }
        }
        sleep 30
    }
}
