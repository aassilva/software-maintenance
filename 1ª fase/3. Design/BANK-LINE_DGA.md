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
6. Visão de Dados
7. Tamanho e Desempenho
8. Qualidade

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
