# Visão Geral

## Estrutura de diretórios

### /

    - Diretórios raiz.
      - Como se fosse o Disco Local (c:)
***

### /bin

    - Diretório de binários.
        - Aqui fica praticamente todos os comandos de gerência do sistema.
    - O /sbin é igual, mas é usado para separar os comandos de configurações, de rede, principalmente.
***

### /boot

    - Inicializador do sistema, aonde o grub fica e o kernel.
***

### /cdrom

    - Se você tiver um leitor de cd, eles serão montados aqui.
***

### /dev

    - Aqui vai estar a raiz dos seus dispositivos de entrada.  
***

### /etc

    - Nesse diretório fica as configurações dos seus programas...
***

### /home

    - Os diretórios dos usuários são montados aqui.
***

### /lib

    - Aqui fica as bibliotecas usadas pelos comandos do diretório /bin e /sbin.
***

### /media

    - aqui é o diretório padrão em que o sistema monta os seus dispositivos externos, como: pedrive e celular.
***

### /mnt

    - Aqui é o diretório que voce vai usar para montar a imagem de partições do seu hd, ssd, entre outros. com o comando mkdir, mas não é uma regra!
***

### /opt

    - Esse diretório é muito usado para separar/guardar os programas proprietários dos livres, como: google chrome, drivers "proprietários" da placa de vídio, entre outros.
    
    - O sistema operacional GNU/Linux usa os seus proprios programas, open source, que vão estar contido na nuvem. Você vai conseguir acessar eles via links que apontam para esses sevidores. Esses links são comunmente chamados de "repositórios", mas eles são somente o link que aponta aos servidor repositórios, aonde contém praticamente todos os programas que você esta usando no linux.
***

### /proc

    Arquivos criados no momento de execução de programas são postos aqui.
***

### /root

    - Diretório do administrador.
***

### /run

    - Assim como o proc, ele guarda dados volateis em que o arquivo está execultando naquele momento.
***

### /snap

    - Como se fosse o diretório opt, mas aqui guarda os arquivos baixados em formato snap, pegos na snapstore
  
    - Existem três "famosos" tipos de instalação no linux. apt, flatpak e snap. O flatpak e o snap são iguais maquinas virtuais, porque os programas são execultados somente em seu seus espaços.
***

### /srv

    - arquivos de servidores...
***

### /usr

    - Dizem que antigamente era a pasta padrão do usuário (home), agora ele guarda binários e outras coisas, tambeḿ.
***

### /var

    - aqui é guardados arquivos que variam com o tempo, tipo logs... e também é aqui que o diretório padrão do seu servidor apache é criado.
