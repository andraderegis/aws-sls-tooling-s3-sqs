<h1 align="center">AWS Lambda - Tooling-S3-SQS</h1>

# Sobre
**Este projeto tem como objetivo a utilização do plugin serverless-offline do framework Serverless. Assim, podemos executar localmente nossas aplicações simulando um ambiente de produção na AWS, evitando custos desnecessários com deploys na AWS Lambda.**

# Scripts
## Package.json
- **start** 
: na declaração desse script, utilizamos o comando **"npx"** à frente do **nodemon** com o intuito de ignorar instalações locais do **nodemon**, sendo que o mesmo é buscado na pasta **node_modules** da aplicação
```
yarn start
```
- **offline**
: inicialização da aplicação, via **serverless**, utilizando o plugin **serverless-offline**. Foi definido o **host como 0.0.0.0** pela necessidade do **docker** realizar mapeamento desse host e, assim, receber requisições externas
```
yarn offline
```