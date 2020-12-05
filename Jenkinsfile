node('ansible-label'){
 stage("clone"){
  checkout scm
 }
 stage("playbook"){
  ansiblePlaybook disableHostKeyChecking: true, inventory: 'hosts', playbook: 'install/nagios.yml'
 }

}
