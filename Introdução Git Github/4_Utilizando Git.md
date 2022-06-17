<img src="C:\Worspace\dio-desafio-github-primeiro-repositorio\Introdução Git Github\imagens\giticon.png" alt="git" style="zoom:25%;" /> ------------ init------ add-------commit------------------

-->	--------------------------------------->   <img src="C:\Worspace\dio-desafio-github-primeiro-repositorio\Introdução Git Github\imagens\githubicon.png" alt="github" style="zoom: 67%;" /> 



Com o GIT instalado é necessário iniciar os comandos

**git init** cria uma pasta oculta dentro do diretório, onde todo processo do GIT irá acontecer

**git add *** inclui todos os arquivos para área de Stage (ficam prontos para serem enviados ao repositório)

**git commit -m "mensagem explicativa do envio"** empacota os arquivos na área de Stage juntamente com a mensagem explicativa

**git push origin master** envia os arquivos para o Github no repositório já devidamente criado



Para melhor entendimento do que o GIT faz, é necessário visualizar o fluxo dos comandos e como o GIT enxerga os arquivos após cada um deles:

![fluxoGit](C:\Worspace\dio-desafio-github-primeiro-repositorio\Introdução Git Github\imagens\fluxoGit.png)



Para trazer repositórios do Github para dentro do seu ambiente:

- **git pull origin master** traz o repósitorio que ja esta sendo trabalhado dentro do seu ambiente

- **git clone {endereço http do repositório disponível no github}** traz um repositório novo