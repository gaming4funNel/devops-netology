# devops-netology
test 1
add for fix branch
with GUI

# Local .terraform directories
**/.terraform/* - все папки .terraform в локальной директории.

# .tfstate files
*.tfstate - файлы с расширением .tfstate.
*.tfstate.* - файлы с расширением .tfstate. и любое другое после точки.

# Crash log files
crash.log - файлы с именем crash.log
crash.*.log - файлы с именем crash. и любое другое после точки.

# Exclude all .tfvars files, which are likely to contain sensitive data, such as
# password, private keys, and other secrets. These should not be part of version 
# control as they are data points which are potentially sensitive and subject 
# to change depending on the environment.
*.tfvars - файлы с расширением .tfvars
*.tfvars.json - файлы с расширением .tfvars.json

# Ignore override files as they are usually used to override resources locally and so
# are not checked in
override.tf - файл override.tf
override.tf.json - файл override.tf.json
*_override.tf - все файлы оканчивающиеся на _override.tf
*_override.tf.json - все файлы оканчивающиеся на _override.tf.json

# Include override files you do wish to add to version control using negated pattern
# !example_override.tf - исключены все файлы example_override.tf

# Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan
# example: *tfplan*

# Ignore CLI configuration files
.terraformrc - файл .terraformrc
terraform.rc - файл terraform.rc