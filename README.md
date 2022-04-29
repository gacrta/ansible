## ALURA ANSIBLE

Projeto do curso https://cursos.alura.com.br/course/infraestrutura-como-codigo-com-ansible

Provisioning é feito via roles especificas:
- `mysql` para instalaçao do banco de dados
- `webserver` para instalação de dependencias do worpress
- `wordpress` para instalação e configuração do wordpress

Dentro das roles:
- `files` possuem os aquivos copiados ou usados em templates
- `handlers` possuem definição dos handlers
- `meta` possui a definição de dependencias
- Por fim, `tasks` possui a listagem das tasks

Para rodar: vagrant@ubuntu-bionic:~$ ansible-playbook /ansible/provisioning.yml -i /ansible/hosts