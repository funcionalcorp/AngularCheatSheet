# Angular Cheat Sheet
Colas para Angular, instalação, configuração, conceitos e comandos frequentes

# Instalação

### 1. NodeJS (Vem com NPM)
O nodeJS é necessário porque vem com/roda o NPM que é o gerenciador de pacotes do Angular.
https://update.angular.io/ 

### 2. Typescript 
Typescript é a linguagem oficial do Angular, criada pela Microsoft, pode ser instalado facilmente através do NPM. Utilize o comando abaixo para instalar:
* npm install -g typescript

### 3. Angular CLI (Command line interface) (NG)
É a linha de comando do angular, não é obrigatória, porém, essencial, pois, gera códigos de templates. Não se preocupe são menos de 10 comandos utilizados e fáceis de se decorar. Utilize o comando abaixo para instalar:
* npm install -g @angular/cli


### 4. Variáveis de ambiente
Pode ser que de acordo com o seu S.O., você precise adicionar o node/ts/ng nas variáveis de ambiente para poder utilizar com mais fácilidade em qualquer diretório da sua linha de comando.
* NPM: Path -> adicionar " ; c:\users\SEUUSUARIO\appData\roaming\npm"

### 5. Confira se tudo está instalado corretamente
Todas as CLIs possuem verificação de versão, utilize para verificar se está tudo instalado, se não retornar a versão então faltou algo.
* ts -v
* npm -v
* ng -v

### 6. Instale a sua IDE
Recomendo utilizar o visual studio code, pela maioria dos conteúdos também utilizarem a mesma IDE
* https://code.visualstudio.com/ 
* Recomendo baixar uma extensão para os ícones das pastas
* Tambem é possível mover a pasta para a direita
* Existem plugins para TFS, porém, são bem fracos apenas checkin e get. As demais operações recomendo utilizar o Visual Studio normal.

### 7. Crie sua solução ou baixe uma existente
Para criar uma solução, crie um diretório e na linha de comando utilize o comando abaixo do ng para criar toda a estrutura padrão: 
* ng new NOMEDASOLUCAO

Caso queria abrir uma solução existente, você pode baixá-la utilizando os plugins do GIT, caso seja TFS recomendo baixar por fora. Então com a solução já baixada, baixe as referencias de packages do projeto utilizando o comando abaixo:
* npm install

Finalmente rode o seu projeto com o comando abaixo
* ng serve


### Demais fontes
* https://angular.io/api (Documentação da API)
* https://angular.io/guide/cheatsheet (CheatSheet do Angular)
* https://loiane.training/course/angular/ (Curso em Portugues gratuito)
* https://docs.npmjs.com/getting-started/what-is-npm (Curso NPM completo Inglês)
* https://update.angular.io/ (Guias para atualizar a versão do angular do seu projeto)


### Repositório de exemplos e técnicas
* https://github.com/funcionalcorp/Angular6DynamicForm (Formulários dinâmicos)
