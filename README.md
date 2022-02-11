# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?

playbook/group_vars/all/examp.yml

2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

ansible-playbook site.yml -i inventory/test.yml

3. Какой командой можно зашифровать файл?

ansible-vault encrypt el/examp.yml

4. Какой командой можно расшифровать файл?

ansible-vault decrypt el/examp.yml

5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? 

Да, можно посмотреть содержимое зашифрованного файла

Если можно, то как?

ansible-vault view group_vars/deb/examp.yml

6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?

команда для ввода пароля в консоле
ansible-playbook site.yml -i inventory/prod.yml --ask-vault-password

команда для чтения пароля из файла
ansible-playbook ansible-playbook secret.yml --vault-password-file=password_file --vault-password-file=password_file

7. Как называется модуль подключения к host на windows?

ansible_connection: winrm

8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh

ansible-doc -t connection ssh

9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?

remote_user

