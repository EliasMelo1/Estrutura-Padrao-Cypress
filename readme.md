# Cypress + Joi 
Projeto de exemplo para realização de testes de API automatizados utilizando o Cypress + Joi

## Ferramentas
- [VSCode](https://code.visualstudio.com/ "VSCode")
- [Joi](https://www.npmjs.com/package/@hapi/joi "Joi")
- [Cypress](https://www.npmjs.com/package/cypress "Cypress")

## Para executar este projeto na sua máquina
  Abra terminal que aceite commandos git (Powershell/git bash/cmder)
  Git clone (ssh/http)
  **Instalar as denpendecias:**
  ```
  npm install
  ``` 
## Tutorial, Instalação e execução


### Para iniciar um novo projeto utilizando está estrutura
* Dentro da pasta especifica para o projeto: 
```
npm init -y
``` 

* Instalar a última versão do Cypress, Joi:
```
npm install cypress @hapi/joi -D
```


* Em um terminal execute o comando abaixo para abrir o cypress:
```
cypress open 
```

### Trick

* Você pode abrir o projeto utilizando o `npx`:
```
npx cypress open
```

### Suites

* Rodar filtrando por suítes:
```
npm run cypress:run -- --env grep=@e2e
```

### Estrutura de pastas:
    | Fixtures: configurações avançadas
    | package-lock.json: configurações avançadas
    | integration: nesta pasta colocamos os nossos arquivos com os cenários de teste escritos no formato BDD.
    | plugin/index.js: este arquivo é destinado para configuração de plugins. Utilizamos ele ao configurar o Cucumber.
    | support: dentro desta pasta colocamos os steps, os scripts e o mapeamento de elementos de nossos testes.
        | commands.js
        | 
    | node_modules: aqui ficam os arquivos de funcionamento do Cypress e do Cucumber. Normalmente não precisamos mexer nesta pasta.
    | cypress.json: neste arquivo podemos realizar configurações globais do nosso projeto. Ex.: criar variáveis globais, 
       definir resolução do navegador, setar uma URL padrão, entre outros.
