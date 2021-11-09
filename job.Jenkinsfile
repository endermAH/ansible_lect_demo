REPO_URL = "https://github.com/endermAH/ansible_lect_demo.git"
PLAYBOOK_PATH = "playbook.yaml"
INVENTORY_PATH = "hosts"

node {
  stage("Clean workspace") {
    cleanWs()
  }
  stage("Clone repo") {
    git REPO_URL
  }
  stage("Run ansible") {
    sh "ansible-playbook ${PLAYBOOK_PATH} -i ${INVENTORY_PATH}"
  }
}
