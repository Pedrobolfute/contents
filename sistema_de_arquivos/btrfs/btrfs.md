# Sistema de arquivo BTRFS

- Umas de suas funcionalidades são:

  - Ele tem mais segurança na transferência de arquivos.
    - Porque ele é baseado na CoW, Copy on Write, ou seja, quando for transferir um arquivo de um lugar para outro, ele vai copiar o arquivo e escrever no local de destino. Assim se houver falha de transferência o arquivo não é totalmente perdido/corrompido.
  - Fácil e mais rápido para criar snapshots.
    - São pontos de restauração do Sistema/Dados. Ou seja, uma cópia confiável do(s) arquivo(s), por precaução.
  - Ele é mais optimizado.
    - Além de empacotar os arquivos ele os compacta para dar mais espaço no HD/SSD.
  - Esse sistema de arquivo é mais flexível.
- Esse sistema de aruqivos é melhor para servidores, por ser flexível e ter mais confiabilidade da transação de dados.
