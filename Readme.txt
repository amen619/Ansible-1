This project to practise Ansible from Jeff Geerling's : DevOps with Ansible.
ssh-key-id: $DO_SSH_KEY

#Found the ssh key using a api request

curl -X GET -H "Content-Type: application/json" -H "Authorization: Bearer $DO_API_TOKEN" "https://api.digitalocean.com/v2/account/keys"

