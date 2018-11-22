install-docker
=========

Role do Ansible para instalação do Docker e Docker Compose em um servidor.

Distribuições Suportadas pela Role
------------

- Debian Jessie ou superior
- RedHat ou CentOS


Tags da Role 
--------------

- deps: Instala as dependências do Docker.
- repo: Insere o repositório do Docker.
- docker: Realiza a instalação do pacote do Docker.
- compose: Realiza a instalação do Docker Compose.


Variáveis da Role 
--------------

Examplos de Playbook
----------------

Exemplo de uso da Role:

    - hosts: servers
      roles:
         - install-docker

License
-------

BSD
