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
- -l (listar)
- -ll (listar com mais detalhes)
- -lh (listar mostrando o tamanho do arquivo em mb, gb)
- -a (listar arquivos acultos)

## Caminho relativo
    - Navergar de diretório em diretório. EX:
  
    - cd /home
    - cd /home/user
    - cd /home/user/documents

## Caminho absoluto
    - Ir direto ao diretório desejado... Ex:
  
    - cd /home
    - cd /home/user/documents


# **Limpar terminal**


## clear
    - Comando para limpar o terminal

## Ctrl + L
    - Tecla de atalho para limpar o terminal


# **Copiar arquivos**


## cp
    - Copia os arquivos para outro diretório... Ex:
     
    - cp /home/user/documents/arquivo1 /home/user/desktop
- -r (recursividade)
- -l (link simbólico absoluto)


# **Mover ou renomear arquivo**


## mv
    -   Comando que move ou renomeia arquivo... EX:
       
    -   mv /home/user/desktop /home/user/downloads
    -   mv -v /home/user/downloads /home/user/desktop
    -   mv -v -f /home/user/desktop /home/user/documents
-   -v (verbosidade/acontecimento em realtime)
-   -f (force/forçar fazer alguma coisa)
-   -i (interative/pergunta antes de sobreescrever arquivo)


# **Criar e remover pastas**


## mkdir
    -   Cria pasta/diretório. EX:
       
    -   mkdir pastaTeste
    -   mkdir -m pastaTesteComPermissao
    -   mkdir -p pai/filho/neto   
-   -m (define permissões)
-   -p (cria subdiretórios também)

## rmdir
    -   Remove as pastas/diretórios. EX:
       
    -   rmdir -p pai/filho/neto
    -   rmdir pastaTesteComPermissao
-   -p (remove parentes/subdiretórios)


# **Criar, remover e ver arquivos**


## touch, gedit, vim, vi, pluma, nano...
    -   Esses comandos acima, com exceção do touch, são editores de textos. O touch além de criar um arquivo vazio, ele manipula metadados dos arquivos. EX:
       
    -   nano novoarquivo
    -   pluma novoarquivo1

## rm
    -   Comando que exclui arquivos, mas também pode excluir diretórios com a opção -r. EX:
       
    -   rm novoarquivo1
    -   rm -r pai
-   -r (recursividade)
-   -v (verbosidade/realtime)
-   -f (force)

## cat
    -   Mostra na tela do terimnal o conteúdo do arquivo, sem precisar acessálo. EX:
       
    -   cat novoarquivo


# **Expressões regulares**


    -   Pode ser usado na estrutura/expressão do comando.  
## *, ?, \\, |, "" 
-   \* = tudo/todas
-   \? = qualquer caractere
-   \\ = o próximo caractere é "especial", como um espaço em branco...
-   | = rodar um comando dentro de outro comando.
-   "" = string; isso tudo é junto.


# **Busca de arquivos**


## find
    -   Comando para procurar arquivos em geral... EX:
       
    -   find /home -ls -iname novoarquivo
    -   find /home -ls -iname *arquivo
-   -iname (nome do arquivo com "i", inclui maiusculo e minusculo)
-   -ls (listagem detalhada)
## grep
    -   Esse comando é muito usado com o find, através da expressão regular "|". Ele serve para filtrar mais ainda suas buscas, ajudando como um marca texto. EX:
       
    -   ls -l | grep "arquivo"
    -   find /home -iname *arquivo | grep arquivo
-   -A (after; numero de linhas depois do resultado)
-   -B (before; numero de linha antes do resultado)


# **Outros comandos**


## help
    -   Quando você não sabe os parametros e estrutura do comando você recorre aqui. EX:
       
    -   find --help

## man
    -   O objetivo desse comando é quase igual ao "help" acima, mas ele te da a documentação do comando mais detalhada... Quando o "help" não ajudar, recorra a este comando. Mas se não estiver aqui sua resposta o "google" vai ser seu melhor amigo. EX:

    -   man find
## apropos
    -   Se você não souber o nome do comando, você pode ter o auxilio desse carinha. Você usa o apropos com alguma palavra especifica que possa possuir no contexto desse comando. EX:
      
    -   "Á eu queria criar uma pasta no terminal, mas qual é o comando que eu vou ultilizar para isso?
        texto: Eu quero "criar" uma "pasta" no "terminal"
        contexto: "criar" "diretório" no "terminal"
        filtrando palavras chaves: "criar" e "diretório"
    Ok. Filtrei as palavras chaves do contexdo do comando que quero, então é só usar com o apropos. Lembrando que tem que traduzir a palavra para o inglês, visto que o terminal é em sua maior parte em inglês..."
        -   apropos directory.
        -   apropos create
    Use o grep, para ser mais especifico.
        -   apropos directory | grep create

## chmod
    -   Muda permissão de pastas e arquivos.
       
        -   MODOS: read (ler) 4; write (escrever) 2; execute (execultar) 1; ou +x (execultar), +w (escrever), +r (ler).
            -   "Os modos são uma das forma de atribuir permissões, aonde você pode atribuir separadamente ou somar os somar os modos que desejam atribuir. EX:

            -   Permissões
                -   Ler e escrever: 4 + 2 = 6
                    -   chmod 6 "nome-do-arquivo"
                -   Ler e execultar: 4 + 1 = 5
                    -   chmod 5 "nome-do-arquivo"
                -   Execultar e escrever: 1 + 2 = 3
                    -   chmod 3 "nome-do-arquivo"
                -   Ler, escrever e execultar: 4 + 2 + 1 = 7
                    -   chmod 7 "nome-do-arquivo"

            -   Outra forma de atribuir é com +r, +w ou +x;
                - chmod +x arquivo
                  - "Mais usado, porque atribui permissão de execultar o arquivo."   
                  -OBS: o "-" tira a permissão.                 
                -   Pode ser sado com (u, g, o, a) para atribuir permissões separadamente a usuários, grupos, outros e todos. EX:
                    
                    - chmod u=rwx,g=rx,o=x "arquivo"
                    - chmod a=r "arquivo"

## apt
    -Aptitude, o comando para instalar, atualizar, pesquisar... programas e pacotes.
        Instalar: apt install "programa/pacote"
        Remover: apt remove "programa/pacote"
        Atualizar pacotes/"bibliotecas": apt update
        Atualizar systema: apt upgrade
        Listar pacotes/programas: apt list
            "Pode-se filtrar com expressões regulares e o grep."