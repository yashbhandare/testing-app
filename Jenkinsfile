pipeline {
	agent any
    stages {
        stage('build') {
            steps {
                sh 'echo I am Here!!!!!!!!!!'
                // sh 'docker build -t gitlab.techverito.com:4567/internal/blog-postservice:${BUILD_NUMBER} .'
                // sh 'docker push gitlab.techverito.com:4567/internal/blog-postservice:${BUILD_NUMBER}'
            }
        }
        stage('test') {
            steps {
                // sh './testing.sh'
            }
        }
        stage('Deploy') {
            steps {
                // sh './deploy_production.sh'
            }
        }
    }
    // post {
    //     always {
    //     sh 'docker rmi -f gitlab.techverito.com:4567/internal/blog-postservice:${BUILD_NUMBER}'
    //     // sh 'docker rmi -f gitlab.techverito.com:4567/internal/blog-userservice:${BUILD_NUMBER}'
    //     sh 'docker-compose down'
    //     }
    //     success {
    //     slackSend channel: '#blog_notification',
    //     color: 'good',
    //     message: """"Build for ${currentBuild.fullDisplayName} was SUCCESSFUL.
    //     Build Number: ${BUILD_NUMBER }
    //     Change Commiter: ${env.GIT_COMMITTER_NAME}
    //     Commit ID ${env.GIT_COMMIT_HASH}"""
    //     }
    //     failure {
    //     slackSend channel: '#blog_notification',
    //     color: 'danger',
    //     message: """Build for ${currentBuild.fullDisplayName} FAILED.
    //     Build Number: ${BUILD_NUMBER }
    //     Change Commiter: ${env.GIT_COMMITTER_NAME}
    //     Commit ID: ${env.GIT_COMMIT_HASH}"""
    //     }
    // }
}