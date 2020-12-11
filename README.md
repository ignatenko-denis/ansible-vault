## ansible-vault

[Encrypting content with Ansible Vault](https://docs.ansible.com/ansible/latest/user_guide/vault.html#creating-encrypted-files)

[Vault](https://www.vaultproject.io/)

```sh
# install….

# check version
ansible-vault --version
# should be mesage «ansible-vault 2.9.15»

# open directory with file application.se

# save your password for encrypt/decrypt in file
echo "pwd" > password_file

# encrypt file application.se
ansible-vault encrypt --vault-password-file password_file application.se

# dencrypt file application.se
ansible-vault decrypt --vault-password-file password_file application.se

# delete file password_file
```
