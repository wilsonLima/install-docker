install-docker
=========

Role do Ansible para instalação do Docker e Docker Compose em um servidor.

Distribuições Suportadas pela Role
------------

- Debian Jessie ou superior
- RedHat ou CentOS


Tags da Role 
--------------

- main: Tag a ser utilizada em conjunto com outras tags, se alguma tag for especificada no comando.
- deps: Instala as dependências do Docker.
- repo: Insere o repositório do Docker.
- docker: Realiza a instalação do pacote do Docker.
- compose: Realiza a instalação do Docker Compose.


Variáveis da Role 
--------------

Exemplos de Playbook
----------------

Exemplo de uso da Role:

    - hosts: servers
      roles:
         - install-docker

Exemplo de Comandos
----------------

Comando para executar todas as tasks:

    ansible-playbook -i <caminho_inventario> <caminho_playbook>

Comando para executar a tag "compose" (em caso de uso de tags, a tag "main" é obrigatória):

    ansible-playbook -i <caminho_inventario> <caminho_playbook> --tags "main, compose"
