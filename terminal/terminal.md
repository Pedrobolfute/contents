# **Visão geral da estrutura de diretórios**

## **/**
    - Diretórios raiz.
      - Como se fosse o Disco Local (c:)

## /bin

## **/boot**
    - Inicializador do sistema, aonde o grub "geralmente" fica.

## /cdrom

## /dev

## **/etc**
    - Nesse diretório fica as configurações dos seus programas...

## **/home**
    - Os diretórios dos usuários são montados aqui.

## /lib

## **/media**
    - aqui é o diretório padrão em que o sistema monta os seus dispositivos externos, como: pedrive e celular.
## **/mnt**
    - Aqui é o diretório que voce vai usar para montar a imagem de partições do seu hd, ssd, entre outros. com o comando mkdir, mas não é uma regra!

## **/opt**
    - Esse diretório é muito usado para separar/guardar os programas proprietários dos livres, como: google chrome, drivers "proprietários" da placa de vídio, entre outros.
    
    - O sistema operacional GNU/Linux usa os seus proprios programas, open source, que vão estar contido na nuvem. Você vai conseguir acessar eles via links que apontam para esses sevidores. Esses links são comunmente chamados de "repositórios", mas eles são somente o link que aponta aos servidor repositórios, aonde contém praticamente todos os programas que você esta usando no linux.
## /proc

## **/root**
    - Diretório do administrador.

## /run

## /snap
    - Como se fosse o diretório opt, mas aaqui guarda os arquivos baixados em formato snap, pegos na snapstore
  
    - Existem três "famosos" tipos de instalação no linux. apt, flatpak e snap. O flatpak e o snap são iguais maquinas virtuais, porque os programas são execultados somente em seu seus espaços.

## /srv

## /sys

## /usr

## /var


# **Navegação entre diretórios**

## cd
    - Navegar entre os diretórios...

## pwd
    - Lista o diretório atual.

## ls
    - Lista os arquivos e diretórios
- -l
- -ll
- lh
- a

## Caminho relativo
    - Navergar de diretório em diretório. EX:
  
    - cd /home
    - cd /home/user
    - cd /home/user/documentos

## Caminho absoluto
    - Ir direto ao diretório desejado... Ex:
  
    - cd /home
    - cd /home/user/documentos


# **Limpar terminal**

## clear
    - Comando para limpar o terminal

## Ctrl + L
    - Tecla de atalho para limpar o terminal


# **Copiar arquivos**

## cp
    - Copia os arquivos para outro diretório... Ex:
    - cp /home/user/documentos/arquivo1 /home/user/desktop
- -r
- -l


# **Mover ou renomear arquivo**


## mv
    -   Comando que move ou renomeia arquivo...
-   -v
-   -f
-   -i


# **Criar e remover pastas**

## mkdir
    -   Cria pasta/diretório.
-   -m
-   -p

## rmdir
    -   Remove as pastas/diretórios
-   -p

# **Criar, remover e ver arquivos**

## touch, gedit, vim, vi, pluma...
    -   Esses comando acima, com exeção do touch, são editores de textos. O touch além de criar um arquivo vazio, ele manipula metadados dos arquivos.

## rm
    -   Comando que exclui arquivos, mas pode-se excluir diretórios com a opção -r.
-   -r
-   -v
-   -f

## cat


# **Expressões regulares**

## *, ?, \, |, ""


# **Busca de arquivos**

## find

## grep


# **Outros comandos**

## help

## man

## apropos

## chmod
    -   Muda permissão de pastas e arquivos.
    -   MODOS: read (ler) 4; write (escrever) 2; execute (execultar) 1;

## apt