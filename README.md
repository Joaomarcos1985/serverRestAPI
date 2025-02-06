### Bootcamp serverRestAPI
## Testes de API Rest do manual ao CI/CD
Criação de testes de API utilizando postaman, newman  e newman-htmlextra

## O que é
Este repositorio foi criado para o bootcamp de teste de API Rest.

## Tecnologias utilizadas
- Postman
- Node v22.13.1
- Newman 6.2.1
- newman-reporter-html

## Documentações

- Análise Tecnica: Analise/
- Doc API: [Consulte Swagger](https://serverest.dev/) 


## Como Instalar o Ambiente
- Primeiro instale o Node [baixe aqui](https://nodejs.org/pt/download)
- Segundo: realize a instalação do newman de forma global [baixe aqui](https://www.npmjs.com/package/newman)
 ```
 npm install -g newman
 ```
- Terceiro: realize a instalação das dependências dps relatórios [baixe aqui](https://www.npmjs.com/package/newman-reporter-htmlextra)
  ```
  npm i newman-reporter-htmlextra
  ```

## Como Rodar os Testes

### Pelo Postman web ou Desketop
- Import a colletion environment
- Execute os testes de forma manual ou automatizada

### Pelo Newman
- Abra o console de preferência
- Execute a seguinte linha de comando para rodar os testes
  ```
  newman run Serverrest.postman_collection.json -e ServeRest.postman_environment.json -r cli
  ```
- Execute os dados com relatório
  ```
  newman run Serverrest.postman_collection.json -e ServeRest.postman_environment.json -r cli,htmlextra
  ```
  ### Report
  Se você optou por rodar os testes com o report htmlextra, você gerou um arquivo html com o resultado dos teses e para verificar as validações você pode abrir a pasta **newman** que foi criada no local em que os arquivos se encontram.
  
## Entre em Contato:
Email: joaomarcos.qatester@gmail.com
