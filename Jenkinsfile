def SSH_USER='jenkins'
def HOST='34.68.166.169'
def PATH= '/var/appvol/ortp/file_extracts/app-data-extracts'

node ('') {
        stage ('SSH') {
          sshagent(credentials: ['jenkins']) {
              script {
                      sh "ssh --vvv ${SSH_USER}@${HOST} cd /var/appvol/ortp/file_extracts/app-data-extracts && ls -al"
          sh "whoami"
        }
        stage('Cleaning Up'){
        }
       }
        }
}
