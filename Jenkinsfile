// Run stages only if the branch is master
piepline {
    agent any 
    stages {
        stage('STAGE-1') {
            when {
                branch 'main'
            }
            steps{
                sh "echo STAGE-2 executes if branch is main"
            }
        }

        stage('STAGE-2'){
            when {
                branch 'test'
            }
            steps{
                sh "echo STAGE-2 executes if branch is main"
            }
        }
    }
}
