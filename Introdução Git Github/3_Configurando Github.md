# <img src="C:\Worspace\dio-desafio-github-primeiro-repositorio\Introdução Git Github\imagens\githubicon.png" alt="ícone Github" style="zoom: 50%;" /> Configurando GITHUB/GIT



O GIT é o versionador de código, através dele será possível empacotar os arquivos de forma criptografada podendo assim enviar seguramente para um repositório remoto, onde outras pessoas possam interagir.

Após criar uma conta no GIthub, insira a chave SSH, para que o Github tenha acesso ao seu GIT.

Dentro do GitBash, na pasta raiz digite os seguintes comandos:

- **ssh -keygen -t ed 25519 -C email@email.com** será solicitada uma senha que é gerada na hora da inserção
- **ls** (liste para visualizar o que dentro da pasta), apareceram dois arquivos, o de extensão .pub sera exposto, assim apenas expondo os arquivos desejados
- **cat id_ed25519.pub** o que aparece na próxima linha trata-se da chave SSH, copie para inserir no Github

Dentro da conta do Github, vá em configurações > chave SSH e Token > new key ssh

- nomeie a chave e cole a chave publica fornecida no prompt.
- volte ao Bash
- **eval $(ssh-agent) -s** retornara o numero do pid, esta td certo!
- **ssh -add id_ed25519** pressione enter e deve abrir o navegador para acesso ao Github, criando a conexão e agora esta tudo pronto para iniciar os envios!...ou commits, rsrsr.



# Configurando GIT

- **git config --global user. email email@email**

- **git config --global user.name {colcoar o mesmo nome utilizado no Github}**

  Essas duas configurações vão fazer com que o commit seja enviado com seus dados

  Para qualquer fim, seguem comandos adicionais:

  - **git config --list** irá listar todas as configurações assim podendo visualizar qual emai e name esta cadastrado
  - **git unset user.name(ou email)** assim remove o email e name cadastrado para edição
  - **git remote -v** mostra o endereço do repositório remoto

