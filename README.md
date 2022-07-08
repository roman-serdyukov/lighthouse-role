Lighthouse-role
=========

Роль, которая устанавливает lighthouse. 
Предварительно устанавливает nginx и git, скачивает lighthouse из заданного репозитория в заданную папку, создает простейший файл настроек вебсервера и меняет в nginx.conf пользователя на root.

Requirements
------------

Работоспособность протестирована на Ubuntu 20.04 и Centos 7.


Role Variables
--------------

Возможно изменить следующие параметры:
- Расположение lighthouse
```
lighthouse_location:
```
- Источник скачивания:
```
lighthouse_src:
```

Example Playbook
----------------
```
    - hosts: servers
      roles:
         - { role: lighthouse, when: ansible_system == 'Linux' }
```
License
-------

MIT

Author Information
------------------

Сердюков Роман
reserdukov@gmail.com
