def SSH_USER='jenkins'
def HOST='34.68.166.16'
def PATH= '/var/appvol/ortp/file_extracts/app-data-extracts'

node ('label''){
        stage ('SSH') {
          sshagent(credentials: ['jenkins']) {
              script {
                      sh "ssh -A -t ${SSH_USER}@${HOST} ${PATH}'bash -s' < bash.sh"
          sh "whoami"
        }
        stage('Cleaning Up'){
        }
       }
        }
}
