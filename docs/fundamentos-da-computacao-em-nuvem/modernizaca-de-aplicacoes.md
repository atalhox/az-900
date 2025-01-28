# Modernização de Aplicações e Otimização de Custos  

## 1. Introdução  

A modernização de aplicativos e a otimização de custos são pilares fundamentais da computação em nuvem. 

Ao migrar para a nuvem ou adaptar aplicações já existentes, as organizações podem alcançar maior eficiência operacional, flexibilidade e economia financeira.  

Esta documentação explora os conceitos essenciais, benefícios e práticas relacionadas ao tema, com ênfase nos conteúdos relevantes para o exame AZ-900.  

---

## 2. Objetivo  

- Apresentar os principais aspectos da modernização de aplicativos e como ela se relaciona com a computação em nuvem.  
- Demonstrar estratégias práticas de redução de custos operacionais em ambientes de nuvem.  
- Preparar o estudante para compreender como essas práticas se aplicam no contexto dos serviços do Azure, especialmente no exame AZ-900.  

---

## 3. Público-alvo  

- Estudantes e profissionais iniciantes interessados em certificações Azure.  
- Gestores e desenvolvedores buscando compreender as vantagens da modernização e otimização na nuvem.  
- Empresas interessadas em explorar soluções de redução de custos e melhorias operacionais por meio do Azure.  

---

## 4. Conteúdo  

### 4.1. Modernização de Aplicações  

#### 4.1.1. Definição

Modernização de aplicações refere-se ao processo de atualizar aplicativos legados para aproveitar os benefícios da tecnologia moderna, incluindo:  

- Escalabilidade.  
- Melhoria de desempenho.  
- Integração com serviços em nuvem.  

#### 4.1.2. Abordagens Comuns  

- **Rehost (Lift-and-Shift)**: Migração direta de aplicativos para a nuvem com poucas ou nenhuma modificação.  
- **Refactor**: Ajustes na arquitetura para aproveitar melhor as capacidades da nuvem.  
- **Rearchitect**: Alteração significativa no design do aplicativo para torná-lo nativo da nuvem.  
- **Rebuild**: Recriação do aplicativo do zero utilizando tecnologias modernas.  

#### 4.1.3. Benefícios da Modernização  

- Redução de tempo de inatividade (downtime).  
- Agilidade no desenvolvimento e entrega de novas funcionalidades.  
- Melhor utilização de recursos por meio de serviços gerenciados (ex.: Azure Kubernetes Service, Azure Functions).  

!!! tip "Dica"  
    Use o **Azure App Service Migration Assistant** para avaliar e migrar aplicativos para o Azure com facilidade.  

---

### 4.2. Redução de Custos Operacionais  

#### 4.2.1. Estratégias para Otimização  

1. **Dimensionamento Adequado de Recursos**: Utilize **Azure Advisor** para obter recomendações sobre dimensionamento e economia.  
2. **Automação**: Configure **políticas de desligamento automático** para recursos não utilizados (ex.: máquinas virtuais).  
3. **Pagamentos Baseados em Consumo**: Aproveite o modelo **Pay-As-You-Go** para pagar somente pelos recursos consumidos.  
4. **Uso de Reservas**: Contrate **instâncias reservadas** para obter descontos em recursos de uso contínuo.  

#### 4.2.2. Exemplos de Redução de Custos no Azure  

- **Azure Cost Management + Billing**: Ferramenta para monitorar e controlar gastos.  
- **Azure Hybrid Benefit**: Utilize licenças locais existentes para economizar em máquinas virtuais no Azure.  
- **Spot Instances**: Execute workloads não críticos a custos reduzidos com capacidade excedente.  

!!! warning "Atenção"  
    O monitoramento contínuo é essencial para evitar custos desnecessários. Revise suas implementações regularmente.  

---

## 5. Guia de Uso  

### 5.1. Modernização de Aplicações  
1. Avalie o estado atual de suas aplicações usando ferramentas como o **Azure Migrate**.  
2. Escolha a abordagem de modernização mais adequada (Rehost, Refactor, etc.).  
3. Utilize serviços gerenciados para facilitar o processo (ex.: Azure App Service).  

### 5.2. Otimização de Custos  
1. Acesse o **Azure Cost Management + Billing** para criar relatórios de consumo.  
2. Ative a **recomendação de eficiência de custos** no **Azure Advisor**.  
3. Configure alertas de orçamento para evitar despesas inesperadas.  

---

## 6. Referências  

- Documentação oficial do Azure: [https://azure.microsoft.com](https://azure.microsoft.com)  
- Guia de Estudo AZ-900: [https://docs.microsoft.com/en-us/learn/certifications/exams/az-900](https://docs.microsoft.com/en-us/learn/certifications/exams/az-900)  
- Ferramentas de custo no Azure: [https://learn.microsoft.com/en-us/azure/cost-management/](https://learn.microsoft.com/en-us/azure/cost-management/)  

---

## 7. Anexos  

### 7.1. Tabela de Comparação de Custos (Exemplo)  
| Serviço Azure            | Custo Inicial | Benefícios         | Caso de Uso Ideal                    |
| ------------------------ | ------------- | ------------------ | ------------------------------------ |
| Azure Virtual Machines   | Médio         | Alta Flexibilidade | Workloads legados.                   |
| Azure Kubernetes Service | Alto          | Escalabilidade     | Aplicações baseadas em containers.   |
| Azure Functions          | Baixo         | Economia por uso   | Funções serverless e tarefas curtas. |
