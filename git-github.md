# GIT-GITHUB

Git criado 2005

- Controle de versionamento distribuido;
- Armazenamento em nuvem;
- Trabalho em equipe;
- Melhora do código;
- Reconhecimento

## COMANDOS BÁSICOS 

### Windows  |  Linux/Mac

- cd | cd : Navegar entre as pastas;

- dir | ls : Listas diretórios (pastas);

- mkdir | mkdir : Criar diretório (pastas);

- del/rmdir | rm -rf : Deletar. No **windows**, *del*: para deletar arquivos e *rmdir*: para deletar diretórios;
    - ex.: *del nome_pasta* , deleta os aruivo dentro da pasta.
           *rmdir nome_pasta /S /Q* , deleta pasta.
           *rm -rf nome_pasta* , deleta pasta.

- cls | clear : limpar terminal. No **Linux/Mac**, *CTRL + L* atalho do teclado para a limpeza;

- echo | echo : criar output;
    - ex.: *echo hello > hello.txt* , cria arquivo hello.txt, com a string (texto) hello.

- mv | mv : mover

> ### ***OBS***
>
> *Flags*: Complementos que acrescentam, modificam ou formatam os comandos.
>
> **No Windows**
> *cd ..* : retroceder um nível na navegação;
> *tab* : autocompleta.


## ***SHA1*** : *Algoritimo de encriptação (hash). Conjunto único de caracteres de 40 dígitos.*
echo "Olá mundo" | openssl sha1
*GIT BASH - terminal: **openssl sha1*** , comando para encripitar 40 carcteres.

## 3 TIPOS BÁSICOS DE OBJETOS DO GIT

- **Blobs** : tipo, tamanho, \0, conteúdo. Metadados do GIT;
        *echo "conteudo" | git bash-object --stdin*

- **Trees** : armazena blobs. tipo, tamanho, \0, blob, sha1, <file>;

- **Commits** : tree, parente, autor. Auteração.

## CHAVES SSH E TOKENS

- **Chave SSH** - Git Bash (terminal extendido)
    - ssh-keygen -t ed25519 -c *email_github*
    - cd para o local
    - dir : listar os numeros dos códigos de chaves (privada e pública)
    - cat id_numero.pub (que foi criado acima)(mostra o conteudo)
    - copy
    - gerar no github
    - eval $(ssh-agent -s)
    - ssh-add id_numero_chave_privada