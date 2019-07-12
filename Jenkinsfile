def SSH_USER='jenkins'
def HOST='34.68.166.16'
def PATH= '/var/appvol/ortp/file_extracts/app-data-extracts'

node ('') {
        stage ('SSH') {
          sshagent(credentials: ['jenkins']) {
              script {
                      sh "ssh -A -t ${SSH_USER}@${HOST} cd ${PATH} ls -al "
          sh "whoami"
        }
        stage('Cleaning Up'){
        }
       }
        }
}
