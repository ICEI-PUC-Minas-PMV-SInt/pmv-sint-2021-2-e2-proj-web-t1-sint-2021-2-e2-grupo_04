# Arquitetura da Solução

Definição de como o software é estruturado em termos dos componentes que fazem parte da solução e do ambiente de hospedagem da aplicação.

## Diagrama de componentes

Diagrama que permite a modelagem física de um sistema, através da visão dos seus componentes e relacionamentos entre os mesmos.

Exemplo: 

Os componentes que fazem parte da solução são apresentados na Figura 01.

![image](https://user-images.githubusercontent.com/4424108/136669745-98f22040-ea4d-4ea6-8c50-f1d675bde881.png)

<center>Figura 01 - Arquitetura da Solução</center>

A solução implementada conta com os seguintes módulos:
- **Web App** - Front end do sistema.
   - **Real-time Database** - Base de dados real-time que sera utilizada para o chat.
- **Backend** - Lógicas de negócios , conexão com banco de dados.
   - **Database** - Armazenamento dos dados persistidos.

A imagem a seguir ilustra a o fluxo do usuário em nossa solução. Assim
que o usuário entra na plataforma.

![image](https://user-images.githubusercontent.com/4424108/136693277-a09bf798-fabd-46c9-891f-99bd072c019b.png)

## Tecnologias Utilizadas

Para desenvolvimento será utilizado as seguintes ferramentas e linguagens:

Ide
- **Jetbrains Webstorm**
- **Visual studio code**

Ferramentas
- **Figma**
- **Whimsical**

Linguagem
- **TypeScript 4.x.x**
- **Java 11**

Linguagem de folha de estilo
- **Style Components**
- **Tailwind**

Bibliotecas
- **ReactJS**
- **react-toastify**
- **react-hook-form**
- **react-modal**

Framework
- **Spring Boot**
- **Spring Data**
- **Spring WebFlux**

Backend-as-a-Service (BaaS)
- **Firebase**

Hospedagem
- **Heroku**

Api
- **https://viacep.com.br/ws/${cep}/json/**

## Hospedagem

Foram criados 2 apps no Heroku onde um está associado a branch staging e a outra associada a branch master ambas com deploy automáticos. 
