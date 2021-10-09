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
que o usuário entra na plataforma, ele é apresentado à tela inicial
(Tela 1) onde ele é confrontado com as opões de editar seu perfil ou
então visualizar sua galeria.

Caso ele opte por seguir pelo primeiro caminho (Editar Perfil), ele é
redirecionado para a tela de edição de perfil (Tela 2), onde pode
atualizar seus dados cadastrais. Nessa tela, o usuário também pode
escolher para editar sua foto de perfil. Ao selecionar essa opção, ele é
redirecionado para a Tela 3, onde ele a imagem expandida do perfil do
usuário é mostrado. Ao selecionar a opção para atualizar a imagem, uma
nova janela abre pedindo para o usuário fazer o upload da nova foto.
Assim que o processo termina um pop-up exibe o status para o usuário
(Tela 4) e o usuário é redirecionado para a Tela 2.

Caso o usuário opte seguir pelo segundo caminho (Visualizar Galeria) ele
é redirecionado para a Tela 5 com todas as fotos que o usuário possui. O
usuário pode clicar em um post qualquer para visualizar os detalhes do
post (Tela 6). Nessa tela, ele pode então escolher editar o post, sendo
redirecionado para a Tela 7. Ao editar as informações, o usuário pode
escolher salvar ou deletar o post. Em ambos os casos o status é
notificado para o usuário (Tela 8) e em seguida ele é redirecionado
para a Tela 2.

![Exemplo de UserFlow](img/userflow.jpg)


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
