# BANK-LINE_DGA 

Versão: V1.00

<h1> Documento de Arquitetura de Software</h1>

## 1. Introdução

### 1.1 Finalidade
Este documento oferece uma visão geral arquitetural abrangente do sistema, usando diversas visões arquiteturais para representar diferentes aspectos do sistema. O objetivo deste documento é capturar e comunicar as decisões arquiteturais significativas que foram tomadas em relação ao sistema.

### 1.2 Escopo
Este documento trata da implementação arquitetura do BANK-LINE com base nos diagramas UML acerca dos casos de uso, diagramas de classe, além da visão lógica do sistema com o detalhamento da arquitetura MVC utilizada, no desenvolvimento.

### 1.2 Visão Geral
Esse documento está dividido nas seguintes seções:

1. Introdução
2. Representação da Arquitetura
3. Visão de Casos de Uso
4. Visão Lógica
5. Visão de Implementação
6. Qualidade

## 2. Representação da Arquitetura
![Diagrama](https://github.com/antlisufg/imagens/blob/master/Flowchart0.png)

Na representação acima mostra o funcionamento da arquitetura MVC aplicada no rails, a qual segue os seguintes passos, usuário já logado no sistema escolhe a opção "Consulta de Saldo".

1. A Aplicação (APP) faz uma solicitação para a Controller.
2. A controller manipula a solicitação.
3. O Model retorna os dados para a ação da Controller.
4. A Controller, passa os dados para a View.
5. A View renderiza e retorna os dados para a aplicação.

## 3. Visão de Casos de Uso
O caso de uso fundamental à arquitetura é:
![Diagrama](https://github.com/antlisufg/imagens/blob/master/UseCase%20Diagram1.png)

### 3.1 Realizações de Casos de Uso
![Diagrama](https://github.com/antlisufg/imagens/blob/master/Sequence%20Diagram1.png)

## 4. Visão Lógica
O usuário interage com o sistema através da view, realizando alguma operação no sistema, a view solicita a controller a ação realizada, A controller processa as informações por meio da comunicação com a model e o database, que por sua vez se comunica com o banco de dados, que por conseguinte repassa o resultado da operação solicitada para a view.

### 4.1 Visão Geral

![Diagrama](https://github.com/antlisufg/imagens/blob/master/Flowchart1.png)

O sistema BANK-LINE é uma aplicação desktop construída de acordo com o modelo de arquitetura MVC (model-view-controller).

- A camada de View é responsável pelo front-end, onde é estabelecida a comunicação entre o usuário e a aplicação. A comunicação acontece apenas com a Controller, através de requisições.

- A camada Controller trata da parte que processa cada ação do sistema, como por exemplo, requisições do usuário. 

- A camada de Model representa os dados da aplicação, basicamente na camada Model ocorre o tratamento da escrita, validação e leitura dos dados. Estes dados devem estar descritos pelas regras de negócio do sistema. Assim a Model, armazena se necessário os dados no database, e se comunica com a Controller quando houver necessidade de exibição, e a Controller decidirar em qual view exibir os dados da Model.

## 5. Visão de Implementação

## 6. Qualidade
Com a definição da arquitetura, houve uma independência proporcionada ao dividir em três partes principais a aplicação. O MVC também torna mais simples a manutenção do software, pois sua estrutura de arquivos torna fácil localizar trechos específicos de código.
