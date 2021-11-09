REPO_URL = "https://github.com/endermAH/ansible_lect_demo.git"
PLAYBOOK_NAME = ""

node {
  stage("Clean workspace") {
    cleanWS()
  }
  stage("Clone repo") {
    git REPO_URL
  }
  stage("Run ansible") {
    sh "ansible-playbook $PLAYBOOK_NAME"
  }
}
