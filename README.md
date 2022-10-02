# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?

> ./group_vars/all/examp.yml

2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

```bash
ansible-playbook -i inventory/test.yml site.yml
```

3. Какой командой можно зашифровать файл?

```bash
ansible-vault encrypt {file}
```

4. Какой командой можно расшифровать файл?

```bash
ansible-vault decrypt {file}
```

5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?

```bash
ansible-vault view {file}
```

6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?

```bash
ansible-playbook -i inventory/prod.yml  site.yml --ask-vault-pass
```

7. Как называется модуль подключения к host на windows?

> ansible.builtin.winrm connection

8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh

```bash
ansible-doc --type connection ssh
```

9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?

>remote_user
