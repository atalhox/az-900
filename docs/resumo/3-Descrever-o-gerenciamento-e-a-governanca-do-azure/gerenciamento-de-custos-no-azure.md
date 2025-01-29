# Gerenciamento de Custos no Azure

## 1. Fatores que Podem Afetar os Custos no Azure

Os custos no Azure podem variar dependendo de diferentes fatores, como service types, região, uso de instâncias reservadas ou spot, e escalabilidade da aplicação.

### 1.1. Tipo de Serviço
Diferentes serviços do Azure possuem modelos de preços distintos, dependendo do consumo de recursos.  

- Virtual Machines (VMs): Cobrança baseada em CPU, memória e tempo de uso.  
- Azure Functions (Serverless): Cobrança baseada no número de execuções e consumo de memória.  
- Armazenamento: Preço determinado pelo espaço utilizado e número de operações realizadas.  

!!! info "Info"
    O modelo de cobrança pode ser Pay-as-you-go (pague pelo uso), Reserved Instances (instâncias reservadas) ou Spot Instances, dependendo da necessidade do usuário.

### 1.2. Região
A localização geográfica do datacenter onde os serviços são hospedados pode impactar os custos.  

- Regiões com maior demanda ou custos operacionais elevados (como Europa Ocidental) geralmente são mais caras.  
- Regiões como Leste dos EUA tendem a ter preços mais baixos devido a maior disponibilidade de infraestrutura.  

!!! tip "Tip"
    Escolha regiões mais baratas sempre que possível, desde que não afete a latência da sua aplicação.

### 1.3. Reserved Instances
O Azure oferece descontos de até 72% para empresas que se comprometem a usar um serviço por 1 ou 3 anos.  

- Ideal para workloads previsíveis que rodam continuamente.  
- Aplica-se a Máquinas Virtuais, Banco de Dados SQL, entre outros serviços.  

!!! info "Info"
    Se sua carga de trabalho é constante, as Reserved Instances oferecem economia significativa em comparação ao Pay-as-you-go.

### 1.4. Spot Instances
As Spot Instances permitem executar workloads não críticas com grandes descontos, aproveitando a capacidade ociosa do Azure.

- Menor custo do que VMs padrão.  
- Menos garantias – a VM pode ser interrompida se o Azure precisar da capacidade para outros clientes.  

!!! warning "Warning"
    As Spot Instances são ideais para testes, processamento em lote e simulações, mas não devem ser usadas para workloads críticos.

### 1.5. Escala

O custo dos serviços pode aumentar conforme o uso cresce, mas há formas de otimizar o orçamento:

- Auto Scaling permite ajustar recursos automaticamente conforme a demanda.  
- Planos Gerenciados em serviços como Azure App Service podem reduzir custos.  

!!! tip "Tip"
    Configure auto scaling para evitar pagar por recursos ociosos em horários de baixa demanda.

## 2. Calculadoras

### 2.1. Azure Pricing Calculator  

A Azure Pricing Calculator permite estimar o custo mensal de serviços no Azure com base nos recursos selecionados e na configuração desejada.

### 2.2. Azure Total Cost Ownership (TCO) Calculator  

A Azure TCO Calculator ajuda a comparar os custos da infraestrutura on-premises com o Azure, levando em consideração custos indiretos, como manutenção, energia e administração.

### 2.3. Comparação: Calculadora de Preços vs. Calculadora de TCO  

A Azure Pricing Calculator e a Azure TCO Calculator ajudam a prever custos no Azure, mas têm propósitos diferentes.

| Ferramenta               | Finalidade                                                | Funcionalidades Principais                                                                           | Quando Usar?                                                |
| ------------------------ | --------------------------------------------------------- | ---------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| Azure Pricing Calculator | Estimar o custo mensal de serviços no Azure.              | - Seleção de serviços<br>- Configuração personalizada de recursos                                    | Planejamento financeiro antes da implantação.               |
| Azure TCO Calculator     | Comparar custos entre Azure e infraestrutura on-premises. | - Cálculo de economia a longo prazo<br>- Consideração de custos indiretos como manutenção e energia. | Avaliação de migração da infraestrutura local para a nuvem. |

!!! tip "Tip"
    Use a Azure Pricing Calculator para estimar custos antes da implementação e a Azure TCO Calculator para justificar a migração para o Azure.




## 3. Funcionalidades de Gerenciamento de Custos do Azure

O Azure Cost Management + Billing permite monitorar e otimizar os custos, fornecendo análises detalhadas e recomendações.

### 3.1. Orçamentos
Permite definir limites de gastos e receber alertas caso o consumo ultrapasse valores definidos.  

- Exemplo: Criar um alerta para quando os custos atingirem 80% do orçamento mensal.  

!!! warning "Warning"
    Defina alertas de orçamento para evitar surpresas na fatura ao final do mês.



### 3.2. Recomendações de Economia
O Azure sugere otimizações automáticas de custo, como:

- Reduzir VMs superdimensionadas.  
- Utilizar Reserved Instances para workloads constantes.  
- Remover recursos não utilizados.  

!!! info "Info"
    O Azure Advisor pode gerar sugestões para reduzir custos com base no uso real dos serviços.



### 3.3. Análise de Custos
Ferramenta que permite visualizar relatórios detalhados sobre onde e como os custos estão sendo gerados.

- Divide os custos por projetos, departamentos e equipes.  
- Gera gráficos interativos para facilitar a análise.  

!!! tip "Tip"
    Use a Análise de Custos para identificar gastos excessivos e otimizar a alocação de recursos.



## 4. Finalidade das Marcas (Tags)

As Tags no Azure permitem categorizar recursos para melhorar o controle de custos e a governança.

### Exemplo de Uso
- Adicionar a tag "Projeto: Finanças" em todas as VMs usadas pelo setor financeiro.  
- Criar relatórios para analisar os custos por equipe, projeto ou cliente.  

!!! tip "Tip"
    Use Azure Tags para melhorar a alocação de custos e rastrear despesas de forma organizada.



## 5. Comparação das Funcionalidades de Gerenciamento de Custos

| Funcionalidade                             | Finalidade                                | Benefícios                                                           |
|  | -- | -- |
| Azure Cost Management + Billing        | Monitorar, analisar e otimizar os custos. | Controle financeiro centralizado e insights detalhados sobre gastos. |
| Budgets (Orçamentos)                   | Definir alertas e limites de gastos.      | Previne custos inesperados e mantém controle sobre despesas.         |
| Azure Advisor (Recomendações de Custo) | Sugere otimizações para reduzir gastos.   | Redução automática de custos com base em padrões de uso.             |
| Cost Analysis (Análise de Custos)      | Relatórios detalhados de uso e custos.    | Melhor visibilidade sobre onde os gastos estão sendo gerados.        |
| Tags (Marcas)                          | Organização e categorização de custos.    | Facilita rastreamento de gastos por equipe, projeto ou cliente.      |