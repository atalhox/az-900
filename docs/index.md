Aqui está uma versão refinada do documento para torná-lo mais claro, objetivo e alinhado com o propósito de estudo para o exame AZ-900. Fiz ajustes no formato, removi redundâncias, reestruturei partes para melhor fluidez e destaquei pontos essenciais com **caixas de atenção**.  

---

# Guia Geral  

---

## 1. Introdução  

A certificação **AZ-900: Microsoft Azure Fundamentals** é ideal para profissionais que desejam adquirir conhecimentos introdutórios sobre a plataforma Azure e conceitos de computação em nuvem.  

Ela proporciona uma visão geral dos principais serviços, benefícios e modelos de precificação do Azure, sendo o ponto de partida para quem pretende construir uma carreira na nuvem.  

Este guia fornece uma estrutura clara para auxiliar nos estudos, apresentando os tópicos cobrados no exame de forma organizada.  

---

## 2. Objetivo  

O objetivo deste documento é:  

- Apresentar os conceitos fundamentais da computação em nuvem.  
- Detalhar os serviços principais do Azure.  
- Explicar segurança, compliance, gerenciamento de custos e suporte.  
- Preparar o candidato para o exame AZ-900, utilizando exemplos práticos e estratégias de estudo.  

---

## 3. Público-alvo  

Este material é voltado para:  

- Profissionais de tecnologia iniciantes na computação em nuvem.  
- Estudantes ou profissionais que buscam entender os serviços do Azure.  
- Tomadores de decisão interessados em avaliar os benefícios do Azure para seus negócios.  
- Candidatos à certificação AZ-900.  

---

## 4. Conteúdo  

### 4.1. Fundamentos de Computação em Nuvem  

A computação em nuvem oferece acesso sob demanda a recursos como servidores, armazenamento e aplicativos por meio da internet, eliminando a necessidade de infraestrutura física local.  

##### 4.1.1. Vantagens  
- **Escalabilidade**: Ampliação ou redução de recursos conforme a necessidade.  
- **Elasticidade**: Ajustes automáticos de recursos baseados na demanda.  
- **Agilidade**: Entrega rápida de serviços para atender requisitos de negócios.  
- **Redução de Custos**: Reduz investimentos em infraestrutura física, utilizando um modelo de pagamento por uso.  

##### 4.1.2. Tipos de Nuvem  
- **Pública**: Recursos compartilhados e gerenciados por provedores, como **Azure** ou **AWS**. Ideal para empresas que buscam custo reduzido e escalabilidade.  
- **Privada**: Infraestrutura dedicada a uma única organização, oferecendo maior controle e segurança.  
- **Híbrida**: Combinação de nuvem pública e privada, permitindo flexibilidade e otimização de recursos.  

##### 4.1.3. Modelos de Serviço  
- **Infraestrutura como Serviço (IaaS)**: Fornece servidores, armazenamento e redes virtuais sob demanda. Ex.: **Azure Virtual Machines**.  
- **Plataforma como Serviço (PaaS)**: Ambiente completo para desenvolvimento e implantação de aplicativos. Ex.: **Azure App Services**.  
- **Software como Serviço (SaaS)**: Aplicativos prontos para uso via internet. Ex.: **Microsoft 365**.  

---

#### 4.1.2. Modernização de Aplicações e Otimização de Custos  

##### 4.1.2.1. Modernização de Aplicativos  
- Atualizar aplicações para aproveitar recursos da nuvem, como:  
  - **Azure App Services**: Para hospedar aplicativos web e APIs de forma escalável.  
  - **Azure Kubernetes Service (AKS)**: Para gerenciamento e orquestração de containers.  
- **Benefícios**:  
  - Melhor desempenho e agilidade no desenvolvimento.  
  - Escalabilidade dinâmica conforme a demanda.  
  - Integração simplificada com outros serviços modernos da nuvem.  

##### 4.1.2.2. Redução de Custos Operacionais  
- **Práticas recomendadas**:  
  - **Azure Cost Management**: Ferramenta para monitorar e otimizar os gastos.  
  - **Automatização de desligamentos**: Configuração de horários para encerrar recursos não utilizados, como VMs.  
  - **Instâncias Reservadas**: Contratação com descontos para workloads previsíveis por 1 ou 3 anos.  

!!! tip "Dica"
    Use o **Azure Advisor** para recomendações de desempenho, segurança e custos.  

---

### 4.2. Introdução aos Principais Serviços do Azure  

#### 4.2.1. Cálculo (Compute)  
- **Máquinas Virtuais (VMs)**: Recursos virtualizados para aplicações.  
- **Azure App Services**: Hospedagem de aplicações web e APIs.  
- **Azure Kubernetes Service (AKS)**: Gerenciamento de containers.  

#### 4.2.2. Armazenamento (Storage)  
- **Blobs**: Armazenamento de objetos não estruturados.  
- **Files**: Solução de compartilhamento de arquivos na nuvem.  

#### 4.2.3. Rede (Networking)  
- **Rede Virtual (VNet)**: Criação de redes isoladas na nuvem.  
- **Load Balancer**: Balanceamento de tráfego entre recursos.  

---

### 4.3. Segurança e Gerenciamento de Identidade  

- **Azure Active Directory (Azure AD)**: Gerenciamento de identidade e autenticação.  
- **Controle de Acesso Baseado em Função (RBAC)**: Controle granular de permissões.  
- **Monitoramento e Auditoria**: Ferramentas como **Azure Monitor** e **Azure Security Center**.  

---

### 4.4. Gerenciamento de Recursos e Governança  

- **Grupos de Recursos**: Organização de recursos relacionados.  
- **Azure Policy**: Aplicação de regras de compliance.  
- **Blueprints**: Implantação consistente de padrões e configurações.  

---

### 4.5. Preços e Suporte  

#### 4.5.1. Modelos de Preço  
- **Pay-As-You-Go (consumo)**: Pagamento baseado no uso real dos serviços. Ideal para cargas de trabalho variáveis.  
- **Instâncias Reservadas**: Descontos significativos para recursos contratados por 1 ou 3 anos. Recomendado para cargas de trabalho previsíveis.  
- **Spot Instances (baixa prioridade)**: Custo reduzido para executar workloads não críticos utilizando capacidade excedente.  

#### 4.5.2. Ferramentas de Gestão de Custos  
- **Calculadora de Preços Azure**: Ferramenta para estimar custos com base em serviços planejados.  
- **Azure Cost Management**: Monitoramento e otimização de gastos em tempo real.  

#### 4.5.3. Níveis de Suporte  
- **Suporte Básico**: Gratuito, com acesso à documentação, fóruns e suporte para cobranças.  
- **Suporte Padrão**: Pago, com suporte técnico 24/7 para problemas de produção.  
- **Suporte Profissional e Premier**: Níveis avançados para empresas com demandas críticas, incluindo planejamento e orientação personalizada.  

Se precisar de mais ajustes ou novos exemplos, avise! 😊

!!! info "Informação"
    A certificação AZ-900 não exige conhecimentos aprofundados sobre preços, mas é importante entender os modelos básicos.  

---

## 5. Guia de Uso  

### 5.1. Planeje sua Jornada de Estudo  
- Siga os módulos do [Microsoft Learn](https://learn.microsoft.com/).  
- Dedique de 1 a 2 semanas para revisar cada módulo.  

### 5.2. Pratique no Azure  
- Crie uma conta gratuita no Azure para experimentar serviços como VMs e App Services.  

### 5.3. Faça Simulados  
- Utilize plataformas como **Whizlabs** ou **ExamTopics** para realizar simulados.  

### 5.4. Consolide Conceitos  
- Revise tópicos mais complexos, como segurança e modelos de precificação.  

!!! tip "Dica"
    Realizar laboratórios práticos ajuda a reforçar conceitos teóricos.  

---

## 6. Referências  

- Documentação Oficial Azure: [https://docs.microsoft.com/en-us/azure](https://docs.microsoft.com/en-us/azure)  
- Exemplo de Exame: [https://www.microsoft.com/learning/exam-az-900](https://www.microsoft.com/learning/exam-az-900)  
- Calculadora de Preços Azure: [https://azure.microsoft.com/pricing](https://azure.microsoft.com/pricing)  

---

## 7. Anexos  

### 7.1. Tabela de Tópicos por Área  

| Área                   | Tópicos principais                           | Peso aproximado no exame |
| ---------------------- | -------------------------------------------- | :----------------------: |
| Fundamentos de nuvem   | Modelos de serviço, benefícios, conceitos    |          15-20%          |
| Serviços principais    | Compute, Storage, Networking                 |          30-35%          |
| Segurança e Identidade | Azure AD, RBAC, ferramentas de monitoramento |          20-25%          |
| Governança e Custos    | Azure Policy, custos, suporte                |          20-25%          |

### 7.2. Esquema Visual de Serviços Azure  

![Azure services](assets/img/azure-services.png)
Diagrama dos serviços oferecidos no Azure e suas interações.  

