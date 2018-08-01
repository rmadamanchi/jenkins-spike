#!groovy

echo "Running ${env.BRANCH_NAME}"

if (env.BRANCH_NAME != 'master') {
    stage('Sleep') {
        echo "Sleeping"
        sleep 30
        echo sh(returnStdout: true, script: 'env')
    }
}
