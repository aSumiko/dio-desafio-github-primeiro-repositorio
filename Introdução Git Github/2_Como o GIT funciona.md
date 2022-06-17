#  <img src="C:\Worspace\dio-desafio-github-primeiro-repositorio\Introdução Git Github\imagens\giticon.png" alt="ícone" style="zoom: 25%;" />		Entendendo o GIT



#### Git é um sistema de controle de versão de arquivos distribuído. Através deles podemos desenvolver projetos na qual diversas pessoas podem contribuir simultaneamente no mesmo, editando e criando novos arquivos e permitindo que os mesmos possam existir sem o risco de suas alterações serem sobrescritas.


Basicamente o Git trabalha com SHA1 (*Secure Hash Algoritm*), um algoritmo de encriptação, de 40 caracteres, único, servindo de identificação. Através desses encriptações são gerados os objetos com o qual sera realizada todo o trabalho do GIT.

### Objetos internos do git

- **BLOBS:** É um objeto onde contem os metadados de um arquivo git, junto do seu conteúdo, encriptado no SHA1. Assim háveram os 40 caracteres encriptados mais os dos metadados.
- **TREES:** Armazenam **BLOBS** , contendo metadados e apontando para um **BLOB** ou para outras árvores. A árvore ira montar toda estrutura de onde estão localizados os arquivos.
- **COMMIT:** É o objeto que vai dar sentido a modificação que você faça. Ele aponta para uma **TREE** um parente, sendo o último **commit** realizado antes dele, um autor e a uma mensagem. Um **commit** também possui um timestamp com a hora que foi criado.

![Esquema Objetos GIT](C:\Worspace\dio-desafio-github-primeiro-repositorio\Introdução Git Github\imagens\objetos.png)