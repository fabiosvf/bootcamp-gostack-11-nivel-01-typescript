####  Bootcamp - GoStack 11
# 🚀 Nível 01 - TypeScript

## Sobre

- Esta Api fornece um modelo básico de um projeto utilizando TypeScript apenas para fins didáticos quanto à instalações de bibliotecas e configurações básicas.

---

## Roteiro

- Nesta seção será descrito o roteiro com todos os passos para criação de um projeto simples em Node.js sem a utilização do comando "create-react-app" utilizando o TypeScript.

### Criando o projeto
- Criar uma pasta
- Acessar a pasta em modo terminal
- Criar o arquivo "package.json" com a configuração padrão
```
$ yarn init -y
```
- Abrir a pasta do projeto no Visual Studio Code
```
$ code .
```
### Instalando bibliotecas e editando configurações
- Instalar a biblioteca "typescript" como dependência de desenvolvimento
  - Essa biblioteca tem a função de converter código TypeScript (.ts) em código JavaScript (.js)
  - De acordo com a Wikipedia, em resumo, o **TypeScript** é um superconjunto de JavaScript desenvolvido pela Microsoft que adiciona tipagem e alguns outros recursos a linguagem. A linguagem pode ser usada para desenvolver aplicações JavaScript no lado cliente e lado servidor (Node.js).
```
$ yarn add typescript -D
```
- Instalar a biblioteca "express"
  - Essa biblioteca tem a função de criar um canal de comunicação com outras aplicações afim de fornecer serviços diversos através de uma requisição HTTP utilizando o padrão RESTfull
```
$ yarn add express
```
- Instalar a biblioteca "@types/express" como dependência de desenvolvimento
  - Essa biblioteca tem a função de tipar a biblioteca "express" de forma à permitir que o TypeScript forneça diversos recursos incluindo Tipagem e Intellisense.
```
$ yarn add @types/express -D
```
-  Converter um arquivo TypeScript (.ts) específico em JavaScript (.js)
```
$ yarn tsc src/index.ts
```
- Iniciar o TypeScript no Projeto
  - Esse procedimento irá criar o arquivo de configuração "tsconfig.json" na raiz do projeto.
```
$ yarn tsc --init
```
- Configurar um Diretório Específico para o TypeScript Converter os Arquivos
  - Localize o parâmetro "outDir" e informe um diretório padrão, por exemplo "./dist"
```
...
"outDir": "./dist"
...
```
- Converter todo o TypeScript (.ts) do projeto em JavaScript (.js) no diretório informado no parâmetro "outDir"
```
$ yarn tsc
```
### Guia TypeScript
- [Guia TypeScript](https://www.notion.so/Typescript-5712aeab312d44fcba0aa88895caad36)

---

## Tecnologias utilizadas

#### Dependências de Projeto
- [express](https://yarnpkg.com/package/express)

#### Dependências de Desenvolvimento
- [typescript](https://yarnpkg.com/package/typescript)
- [@types/express](https://yarnpkg.com/package/@types/express)

---

## Como executar
- Crie uma pasta para o projeto
- Acesse a pasta
- Faça o clone do projeto
```
$ git clone https://github.com/fabiosvf/bootcamp-gostack-11-nivel-01-typescript.git .
```
- Atualize as bibliotecas
```
$ yarn
```
- Converta TypeScript em JavaScript
```
$ yarn tsc
```
- Inicie o serviço
```
$ node ./dist/index.js
```