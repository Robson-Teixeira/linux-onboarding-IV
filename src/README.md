## Comandos:
- `sudo useradd robson` para criar um novo usuário chamado "robson"
- `sudo adduser robson` para adicionar um novo usuário chamado "robson" (interativo)
- `cat /etc/passwd | grep robson` para verificar se o usuário "robson" foi criado
- `cat /etc/group` para listar todos os grupos do sistema
    - `cat /etc/group | grep robson` para verificar se o grupo "robson" foi criado
- `cat /etc/shadow | grep robson` para verificar a senha do usuário "robson"
- `groups` para listar os grupos do usuário atual
    - `groups robson` para listar os grupos do usuário "robson"
- `su - robson` para trocar para o usuário "robson"
- `logout` para sair da sessão do usuário atual
- `sudo groupadd projetos` para criar um novo grupo chamado "projetos"
- `sudo usermod -aG projetos robson` para adicionar o usuário "robson" ao grupo "projetos"
- `sudo vi /etc/group` para editar o arquivo de grupos
- `sudo userdel robson` para deletar o usuário "robson"
- `sude groupdel projetos` para deletar o grupo "projetos"
- `ls - l /var` para listar os arquivos e diretórios em /var
- `sudo chmod -R 755 /var` para alterar as permissões de todos os arquivos e diretórios em "/var" para "755" (7 - rwx - usuário com controle total, 5 - r-x - grupo pode ler e executar, 5 - r-x - outros podem ler e executar)
    > File Permissions:
    Dado **drwxrwxrwx** ou **-rwxrwxrws**: Arquivo '**-**', diretório '**d**', ou link simbólico '**l**'.Permissões de leitura '**r**', escrita '**w**' e execução '**x**' para o proprietário, grupo e outros usuários. 
    Representado por números:
    - 7: rwx (leitura, escrita, execução)
    - 6: rw- (leitura, escrita)
    - 5: r-x (leitura, execução)
    - 4: r-- (leitura)
    - 3: -wx (escrita, execução)
    - 2: -w- (escrita)
    - 1: --x (execução)
    - 0: --- (nenhuma permissão)