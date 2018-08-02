#!groovy

echo "Running ${env.BRANCH_NAME}"

if (env.BRANCH_NAME != 'master') {
    stage('Sleep') {
        echo "Sleeping"
        echo new JsonBuilder(currentBuild.toPrettyString()
        sleep 30
    }
}
