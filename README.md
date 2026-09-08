# Car Rental Billing System

Sistema de aluguel de veículos desenvolvido em Java, com processamento de período de locação, cálculo de pagamento e aplicação de impostos.

O projeto foi desenvolvido com foco na prática de conceitos de Programação Orientada a Objetos, organização de responsabilidades e criação de uma estrutura de serviços para processamento de uma fatura de aluguel.

## Funcionalidades

- Cadastro do modelo do veículo.
- Definição da data e hora de retirada e devolução.
- Definição do preço por hora.
- Definição do preço por dia.
- Cálculo do pagamento básico do aluguel.
- Cálculo de impostos.
- Cálculo do pagamento total.
- Geração de uma fatura com os valores calculados.

## Tecnologias

- Java
- Programação Orientada a Objetos
- `LocalDateTime`
- `DateTimeFormatter`
- Collections e classes de domínio
- Organização em pacotes

## Estrutura do Projeto

```text
src/
├── application/
│   └── Program.java
│
└── model/
    ├── entities/
    │   ├── CarRental.java
    │   ├── Invoice.java
    │   └── Vehicle.java
    │
    └── services/
        ├── BrasilTaxService.java
        └── RentalService.java
Principais conceitos aplicados
Programação Orientada a Objetos

O projeto utiliza classes para representar diferentes responsabilidades do sistema, como veículo, aluguel, fatura e serviços de cálculo.

Separação de responsabilidades

A lógica de processamento do aluguel está concentrada na classe RentalService, enquanto o cálculo dos impostos é realizado pelo BrasilTaxService.

Essa organização permite manter as responsabilidades separadas e facilita futuras alterações no sistema.

Manipulação de datas

As classes LocalDateTime e DateTimeFormatter são utilizadas para representar e formatar as datas e horários de retirada e devolução do veículo.

Processamento da fatura

Após receber os dados do aluguel, o sistema processa a cobrança e gera uma Invoice contendo:

Pagamento básico;
Imposto;
Pagamento total.
Fluxo da aplicação
Dados do aluguel
       ↓
Vehicle
       ↓
CarRental
       ↓
RentalService
       ↓
Cálculo do pagamento
       ↓
BrasilTaxService
       ↓
Cálculo do imposto
       ↓
Invoice
       ↓
Resultado final
Como executar
Clone o repositório:
git clone git@github.com:Davi-S1va/car-rental-billing-system.git
Abra o projeto em uma IDE compatível com Java, como Eclipse ou IntelliJ IDEA.
Execute a classe:
src/application/Program.java
Informe os dados solicitados pelo programa no terminal.
Objetivo

Este projeto faz parte da minha evolução no desenvolvimento com Java e tem como objetivo consolidar conhecimentos de Programação Orientada a Objetos, modelagem de entidades, organização de responsabilidades e desenvolvimento de aplicações orientadas a regras de negócio.

Desenvolvido por Davi Silva.


