This project to practise Ansible from Jeff Geerling's : DevOps with Ansible.
ssh-key-id: 26665491

#Found the ssh key using a api request

curl -X GET -H "Content-Type: application/json" -H "Authorization: Bearer 47af7f0689523c62d1716521da79c18b3b318d05d0623bc9ee0956b6e835ed75" "https://api.digitalocean.com/v2/account/keys"

test
