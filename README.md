# Angular Cheat Sheet
Colas para Angular, instalação, configuração, conceitos e comandos frequentes

# 1. Instalação

### 1.1. NodeJS (Vem com NPM)
O nodeJS é necessário porque vem com/roda o NPM que é o gerenciador de pacotes do Angular.
https://nodejs.org/en/download/

### 1.2. Typescript 
Typescript é a linguagem oficial do Angular, criada pela Microsoft, pode ser instalado facilmente através do NPM. Utilize o comando abaixo para instalar:
* npm install -g typescript

### 1.3. Angular CLI (Command line interface) (NG)
É a linha de comando do angular, não é obrigatória, porém, essencial, pois, gera códigos de templates. Não se preocupe são menos de 10 comandos utilizados e fáceis de se decorar. Utilize o comando abaixo para instalar:
* npm install -g @angular/cli

### 1.4. Variáveis de ambiente
Pode ser que de acordo com o seu S.O., você precise adicionar o node/ts/ng nas variáveis de ambiente para poder utilizar com mais fácilidade em qualquer diretório da sua linha de comando.
* NPM: Path -> adicionar " ; c:\users\SEUUSUARIO\appData\roaming\npm"

### 1.5. Confira se tudo está instalado corretamente
Todas as CLIs possuem verificação de versão, utilize para verificar se está tudo instalado, se não retornar a versão então faltou algo.
* ts -v
* npm -v
* ng -v

### 1.6. Instale a sua IDE
Recomendo utilizar o visual studio code, pela maioria dos conteúdos também utilizarem a mesma IDE
* https://code.visualstudio.com/ 
* Recomendo baixar uma extensão para os ícones das pastas
* Tambem é possível mover a pasta para a direita
* Existem plugins para TFS, porém, são bem fracos apenas checkin e get. As demais operações recomendo utilizar o Visual Studio normal.

# 2. Criando uma solução ou abrindo uma existente

### 2.1. Criando uma solução
Para criar uma solução, crie um diretório e na linha de comando utilize o comando abaixo do ng para criar toda a estrutura padrão: 
* ng new NOMEDASOLUCAO

### 2.2. Abrindo uma solução existente
Caso queria abrir uma solução existente, você pode baixá-la utilizando os plugins do GIT, caso seja TFS recomendo baixar por fora (No Visual Studio normal). Então com a solução já baixada, baixe as referencias de packages do projeto utilizando o comando abaixo:
* npm install

### 2.3. Rodando
Finalmente rode o seu projeto com o comando abaixo
* ng serve

# 3. Dicas de utilização

### 3.1. Geral
* Angular é voltado para SPA (Single Page Application), enxergue o index.html e o app-componente principal como sendo equivalente à uma masterPage (webforms) ou Layouts (mvc), os componentes internos podem ser duas categorias: ContentPages(webforms)/Views(MVC) quando dentro de um router-outlet (holder da view), ou pode ser equivalente a usercontrols(webforms)/subviews(mvc). Porém, muito mais maleáveis, dinâmicos e fáceis devido ao fato de serem totalmente client side.
* Todo componente tem por default 4 arquivos: CSS, HTML, TS e Teste unitário. Caso não estejam fazendo os testes unitários apenas ignorar
* Além dos componentes acima, existem os services, são os arquivos que contém as lógicas de negócio do front (Normalmente acessar uma API e fazer algumas operações menores, formatações e manuseações que possam ser necessárias). Normalmente se agrupam os arquivos services em uma pasta para melhor organização.
* Utilize o Angular CLI para criar a estrutura de um projeto e também para criar os seus arquivos (components, services, modules, etc), isso poupa bastante esforço
* Modulos do angular são utilizados para agrupar conteúdos, isto ajuda na organização das referencias e também tem outras utilidades (separação dos pacotes).
* O projeto padrão do angular vem com 2 tipos de padrões de testes:  e2e jasmine (proactor.conf.js) que testa no browser e o karma (karma.conf.js) que é teste unitário, parece ser bem interessante para automação de testes. Parecem ser fáceis, mas ainda não testei muito.
* O angular vem com o tslint que é uma espécie de R# para TS, as configurações ficam no tslint.json
* Mantenha a estrutura de pastas do Angular e tenha bom senso na organização, isto é super importante para a escalabilidade da aplicação, veja esta aplicação exemplo: https://github.com/juniortarcisio/WITP 



# 4. Demais fontes

### 4.1. Links gerais 
* https://angular.io/api (Documentação da API)
* https://angular.io/guide/cheatsheet (CheatSheet do Angular)
* https://update.angular.io/ (Guias para atualizar a versão do angular do seu projeto)
* https://loiane.training/course/angular/ (Curso em Portugues gratuito)

### 4.2. Ferramentas satélites
* https://github.com/angular/angular-cli/wiki (Wiki com CheatSheet do AngularCLI/NG)
* https://docs.npmjs.com/getting-started/what-is-npm (Curso NPM completo Inglês)

### 4.2. Repositório de exemplos e técnicas
* https://github.com/funcionalcorp/Angular6DynamicForm (Formulários dinâmicos)
