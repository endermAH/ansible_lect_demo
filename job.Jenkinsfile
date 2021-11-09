REPO_URL = "https://github.com/endermAH/ansible_lect_demo.git"
PLAYBOOK_NAME = "ansible_lect_demo/playbook.yaml"

node {
  stage("Clean workspace") {
    cleanWs()
  }
  stage("Clone repo") {
    git REPO_URL
  }
  stage("Run ansible") {
    sh "ansible-playbook $PLAYBOOK_NAME"
  }
}
