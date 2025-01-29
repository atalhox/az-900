# Descrever a Computação em Nuvem

## 1. Computação em Nuvem

### 1.1 Definição de Computação em Nuvem

A computação em nuvem é um modelo que permite o acesso onipresente, conveniente e sob demanda a um conjunto compartilhado de recursos de computação configuráveis (como redes, servidores, armazenamento, aplicações e serviços) que podem ser rapidamente provisionados e liberados com o mínimo esforço gerencial ou interação com o provedor de serviço.

## 2. Modelo de Responsabilidade Compartilhada

### 2.1 Descrição

O modelo de responsabilidade compartilhada entre o provedor de serviços em nuvem e o cliente define quem é responsável por quais aspectos da segurança. 

Em geral:

- **Infraestrutura como Serviço (IaaS)**: O cliente gerencia o sistema operacional, aplicações e dados, enquanto o provedor cuida da infraestrutura física.
- **Plataforma como Serviço (PaaS)** e **Software como Serviço (SaaS)**: O provedor gerencia a infraestrutura e também pode gerenciar o sistema operacional e/ou aplicações, enquanto o cliente gerencia os dados e o acesso dos usuários.

## 3. Definir os Modelos de Nuvem: Público, Privado e Híbrido

### 3.1 Modelo Público

Os serviços são entregues através da internet e compartilhados entre vários clientes que usam os mesmos recursos.

### 3.2 Modelo Privado

A infraestrutura é dedicada a uma única organização e não é compartilhada. Pode estar localizada no local (on-premise) ou hospedada por terceiros.

### 3.3 Modelo Híbrido

Combina elementos dos modelos público e privado, permitindo que dados e aplicações se movam entre os dois ambientes.

## 4. Identificar os Casos de Uso Apropriados para Cada Modelo de Nuvem

### 4.1 Público

Ideal para aplicações com demanda variável, desenvolvimento e teste, e serviços que requerem grande escalabilidade.

### 4.2 Privado

Indicado para operações críticas, dados sensíveis e requisitos regulatórios específicos que não podem ser atendidos pelo ambiente público.

### 4.3 Híbrido

Perfeito para empresas que precisam de flexibilidade e controle do ambiente privado, mas querem aproveitar a escalabilidade do ambiente público para aplicações menos sensíveis.

## 5. Descrever o Modelo Baseado em Consumo

### 5.1 Descrição

Este modelo permite que os usuários paguem apenas pelos recursos de computação que realmente usam, geralmente medidos por hora ou por unidade de serviço consumida. Isso contrasta com os modelos de pagamento antecipado ou fixo, proporcionando uma forma mais flexível e econômica de usar os serviços de computação.

## 6. Comparar os Modelos de Preços de Nuvem

### 6.1 Pagamento conforme o uso

Os clientes pagam apenas pelos recursos que utilizam.

### 6.2 Assinaturas

Pagamento fixo mensal ou anual que pode oferecer descontos baseados no compromisso de uso.

### 6.3 Preços Spot/Instâncias Spot

Oferece preços mais baixos para recursos não utilizados, com a condição de que o provedor pode recuperá-los a qualquer momento se precisarem dos recursos para outros clientes.

## 7. Descrever a Computação Serverless

### 7.1 Descrição

A computação sem servidor permite que os desenvolvedores construam aplicações focadas apenas no código que diferencia sua aplicação, sem se preocupar com a gestão da infraestrutura. 

O provedor de nuvem gerencia automaticamente a alocação de recursos, escalando de acordo com a demanda do aplicativo sem intervenção manual.

!!! tip "Dica"
    Explorar a computação sem servidor pode reduzir significativamente os custos operacionais, pois elimina a necessidade de gerenciar servidores e outros recursos de hardware.