def SSH_USER='jenkins'
def HOST='34.68.166.169'
def PATH= '/var/appvol/ortp/file_extracts/app-data-extracts'

node ('') {
        stage ('SSH') {
          sshagent(credentials: ['jenkins2']) {
              script {
                      sh "ssh ${SSH_USER}@${HOST} cd ${PATH}"
          sh "whoami"
        }
        stage('Cleaning Up'){
        }
       }
        }
}
