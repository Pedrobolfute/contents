# Sistema de arquivo

- Define o gerenciamento dos arquivos.
  - Pense o seguinte: para resolver um problema falamos muito em algorítimo (sequencia de passos para resolver o problema). Então o Sistema de arquivos é um algorítimo para resolver/gerenciar arquivos no linux. Pode-se encontrar vários tipos de arquivos, cada um com seu algorítimo e contexto específico.

## Sistema de arquivo ext4

- Uma de suas funcionalidades é...

Ele é mais ultilizado no linux e suporta muitos outros sistemas de arquivos, como os do Windows. Mas sua segurança para transferência não é muito eficaz quanto o btrf, se houver falha no mover um arquivo de um local para outro, esse arquivo pode ser corrompido mais facilmente.

## Sistema de arquivo btrfs

- Uma de suas funcionalidades é...

Ele tem mais segurança na transferência de arquivos. Porque ele é baseado na CoW, Copy on Write, ou seja, quando for transferir um arquivo de um lugar para outro, ele vai copiar o arquivo e escrever no local de destino. Assim se houver falha de transferência o arquivo não é totalmente perdido/corrompido.
