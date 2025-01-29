# Recursos e Ferramentas para Gerenciar e Implantar Recursos do Azure

## 1. Azure Portal

O Azure Portal é uma interface gráfica baseada na web que permite aos usuários visualizar e gerenciar todos os serviços e recursos do Azure. 

Ele oferece um ponto centralizado para criar, configurar, gerenciar e monitorar máquinas virtuais, redes, aplicativos, bancos de dados e mais.

Além disso, o portal exibe métricas de desempenho, permite configurar alertas de estado e gerenciar custos e faturamento.

!!! tip "Tip"
    Use o Azure Portal para tarefas visuais e rápidas, como a criação manual de recursos e configuração de alertas sem precisar de código.

## 2. Azure Cloud Shell

O Azure Cloud Shell é um shell interativo acessível diretamente no navegador, eliminando a necessidade de instalar ferramentas localmente. Ele inclui duas opções:

- Azure CLI (Command-Line Interface): Interface de linha de comando para gerenciar recursos do Azure com comandos simples.
- Azure PowerShell: Coleção de cmdlets que permite gerenciar o Azure de forma programática usando scripts do PowerShell.

O Cloud Shell já vem pré-configurado e autenticado, tornando mais fácil executar scripts sem necessidade de configurar credenciais manualmente.

!!! info "Info"
    O Cloud Shell mantém arquivos e configurações persistentes usando um Armazenamento do Azure, garantindo que scripts e configurações não sejam perdidos entre sessões.

## 3. Azure Arc

O Azure Arc permite gerenciar servidores, Kubernetes, bancos de dados e serviços fora do Azure, incluindo ambientes on-premises e outras nuvens como AWS e Google Cloud.  

Ele traz a experiência de gerenciamento do Azure para qualquer infraestrutura, possibilitando controle centralizado e aplicação de políticas de segurança e compliance de forma unificada.  

### 3.1. Principais Recursos do Azure Arc  

- Gerenciamento Unificado: Administre recursos locais e multinuvem diretamente do Azure Portal, como se fossem nativos do Azure.  
- Automação e Segurança: Aplique políticas de segurança consistentes e automatize a governança em ambientes híbridos.  
- Extensão de Serviços do Azure: Use Azure Monitor, Microsoft Defender for Cloud e Azure Policy em infraestruturas externas.  

### 3.2. Exemplo  

Uma empresa que possui 100 servidores físicos on-premises e 50 VMs na AWS pode registrar esses servidores no Azure Arc.  

- A equipe de TI pode monitorar métricas de desempenho e aplicar atualizações de segurança diretamente do Azure Portal, sem precisar acessar cada ambiente individualmente.  
-O Microsoft Defender for Cloud pode ser ativado nesses servidores externos, protegendo-os contra ameaças de segurança.  

#### Kubernetes Multicloud com Azure Arc  

Uma startup executa aplicativos em Amazon EKS (Elastic Kubernetes Service) e Google Kubernetes Engine (GKE), mas deseja padronizar o gerenciamento dessas cargas de trabalho.  

- Com o Azure Arc-enabled Kubernetes, a empresa pode aplicar políticas de segurança uniformes em clusters Kubernetes de diferentes provedores de nuvem.  
- Permite implantar Azure Policies e Azure Monitor para visualizar logs e métricas em um único painel centralizado no Azure.  

!!! tip "Tip"
    O Azure Arc for Kubernetes simplifica a gestão de clusters espalhados em diferentes provedores de nuvem, permitindo que todos sejam governados como se estivessem dentro do Azure.

!!! warning "Warning"
    O Azure Arc exige registro dos recursos externos para que possam ser monitorados e gerenciados como parte da infraestrutura do Azure.

## 4. Infrastructure as Code (IaC)

A Infraestrutura como Código (IaC) permite gerenciar e provisionar recursos de TI por meio de código, evitando configurações manuais e melhorando a consistência. 

No Azure, as principais ferramentas para IaC incluem:

- Azure Resource Manager (ARM) – Nativo do Azure, permite automação por meio de templates JSON.
- Terraform – Ferramenta de código aberto amplamente utilizada para criar infraestrutura multicloud.
- Pulumi – Alternativa moderna ao Terraform que permite definir infraestrutura usando linguagens de programação convencionais.

!!! tip "Tip"
    Adote IaC para criar ambientes consistentes, eliminando erros manuais e garantindo desempenho previsível em implantações repetitivas.

## 5. Azure Resource Manager (ARM) e ARM Templates

O Azure Resource Manager (ARM) é a camada de gerenciamento e implantação do Azure que permite organizar e controlar recursos. 

Ele facilita:

- Gerenciamento em grupos para aplicação de políticas e controle de acesso.
- Implantações consistentes e automatizadas com ARM Templates.
- Atualizações sem downtime através de modelos declarativos.

Os ARM Templates são arquivos JSON que definem recursos e dependências, permitindo a implantação repetível e escalável de ambientes complexos.

!!! info "Info"
    O Azure Bicep é uma alternativa ao ARM Templates, fornecendo uma sintaxe mais legível e simplificada para criar definições de infraestrutura no Azure.
