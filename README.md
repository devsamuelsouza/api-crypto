# API Crypto

Esse projeto consiste em uma api com o intuito de obter a cotação das criptomoedas mais populares em tempo real.

## 📋 Pré-requisitos

Para utilizar esse projeto de forma local você precisará atender aos seguintes requisitos:

- [Git](https://git-scm.com/downloads) para instalar o projeto.
- [Docker](https://www.docker.com/) para rodar o container.
- [CoinMarketCap](https://coinmarketcap.com/) para obter a chave da API.

## 🔧 Instalação

Siga esse passo a passo para instalar o projeto:

- Instale o Git  clicando [aqui.](https://git-scm.com/downloads) 
- Abra o Terminal (CMD, PowerShell ou Git) na pasta onde deseja instalar o projeto
- Digite os seguintes comandos 

```bash
    git clone https://github.com/devsamuelsouza/api-crypto.git 
```

```bash
    cd api-crypto
```

## 📦 Implantação

Para implantar o projeto em sua maquina, siga os seguintes passos:

- Abra o terminal (CMD, PowerShell ou Git) no diretorio raiz do projeto
- Renomeie o arquivo .env.example

```bash
    mv .env.example .env
```

- Adicione ao arquivo .env sua API Key e a porta em que deseja rodar a aplicação

- Digite o seguinte comando para criar a imagem no Docker

```bash
    docker build -t api-crypto . 
```

- Após isso, crie o container que irá rodar o projeto

```bash
    docker run -p "PORTA_ESCOLHIDA":3333 -d api-crypto
```

## **🧪 Testes**  

Verifique o funcionamento do sistema realizando os seguintes testes:  

- **Envio da requisição:** A requisição deve ser enviada através do método GET para a seguinte rota.

```bash
    http://localhost:PORTA_ESCOLHIDA/cotacao/coins
```

- **Verifique sua conta da CoinMarketCap** Verifique a quantidade de requisições disponiveis.

- **Envio de requisições para outras rotas:** Verifique se ao acessar uma rota invalida, a mesma retorna uma menssagem de erro.

*Dica:* Explore possíveis erros ou melhorias na aplicação.  
*Obs:* A aplicação aceita apenas requisições do tipo GET

## **📡 Online**

- Caso queira acessar API de forma online, envie a requisição para:

```bash
    https://api-crypto-q3f7.onrender.com/cotacao/coins
```

## **🛠️ Tecnologias e Ferramentas Utilizadas**  
Este projeto foi desenvolvido utilizando as seguintes tecnologias e ferramentas:  

![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![Nodemon](https://img.shields.io/badge/NODEMON-%23323330.svg?style=for-the-badge&logo=nodemon&logoColor=%BBDEAD)
![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white)
![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=for-the-badge&logo=express&logoColor=%2361DAFB)
![NPM](https://img.shields.io/badge/NPM-%23CB3837.svg?style=for-the-badge&logo=npm&logoColor=white)
![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)

## **📌 Versão**  

Consulte as [tags neste repositório](https://github.com/devsamuelsouza/api-crypto/tags) para visualizar as versões do projeto.

## **✒️ Autor**  
Desenvolvido por **Samuel Souza** 🌹  
- [GitHub](https://github.com/devsamuca)  
- [LinkedIn](https://www.linkedin.com/in/devsamuel/)  

---