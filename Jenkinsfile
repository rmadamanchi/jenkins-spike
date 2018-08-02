#!groovy

echo "Running ${env.BRANCH_NAME}"

if (env.BRANCH_NAME != 'master') {
    stage('Sleep') {
        echo "Sleeping"
        currentBuild.dump()
        sleep 30
    }
}
