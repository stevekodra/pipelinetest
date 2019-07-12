def SSH_USER='jenkins'
def HOST='34.68.166.16'
def PATH= '/var/appvol/ortp/file_extracts/app-data-extracts'

node ('TOOLING_LINUX_GBL20039993') {

        stage ('SSH To Cognos') {
          sshagent(credentials: ['jenkins']) {
              script {
          sh "ssh -A -t ${SSH_USER}@${HOST} 'bash -s' < bash.sh"
          sh "whoami"
        }
        stage('Cleaning Up'){
        }
       }
    }
  }
