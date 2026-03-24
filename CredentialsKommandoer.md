#krypter og dekrypter filer
ansible-vault encrypt credentials.yml

ansible-vault decrypt credentials.yml

#krypter og dekrypter fstrings/variabler
ansible-vault encrypt_string 'DatabasePassword123' --name 'db_password' --encrypt-vault-id default

ansible-vault encrypt_string 'sk-1234567890abcdef' --name 'api_key' --encrypt-vault-id default

ansible-vault encrypt_string 'Admin@Pass2024' --name 'admin_password' --encrypt-vault-id default

---
# Database credentials
mysql_host: 10.1.0.6
mysql_user: dbadmin
mysql_password: PlainTextPassword123

# AWS credentials
aws_access_key: AKIAIOSFODNN7EXAMPLE
aws_secret_key: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
