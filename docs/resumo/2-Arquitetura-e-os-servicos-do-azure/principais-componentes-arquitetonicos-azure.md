## Principais Componentes Arquitetônicos do Azure

### 1. Regiões do Azure, Pares de Regiões e Regiões Soberanas

#### 1.1 Regiões do Azure

Regiões do Azure são áreas geográficas específicas onde os datacenters estão localizados, otimizados para redundância e baixa latência.

!!! info "Info"
    Uma região do Azure pode conter múltiplos datacenters, mas todos dentro de uma mesma jurisdição para cumprir requisitos legais e de conformidade.

!!! info "Exemplo" 
    Região Leste dos EUA (East US): Localizada em Virginia, esta região é um dos centros mais populares devido à sua proximidade com grandes centros de negócios na costa leste dos Estados Unidos. Empresas de tecnologia e grandes corporações frequentemente escolhem esta região para otimizar a entrega de serviços aos seus usuários na América do Norte.

#### 1.2 Pares de Regiões

Cada região é emparelhada com outra região próxima para possibilitar a recuperação de desastres e manter a continuidade dos serviços.

!!! tip "Dica"
    Par de Regiões: Leste dos EUA e Oeste dos EUA: O Leste dos EUA (Virginia) é frequentemente emparelhado com o Oeste dos EUA (Califórnia), permitindo que as empresas implementem estratégias de failover e de recuperação de desastres ao espelhar seus dados e serviços entre estas regiões geograficamente dispersas.

!!! info "Exemplo"
    Serviço de streaming de vídeo: Uma plataforma de streaming pode usar regiões emparelhadas para garantir que, mesmo em caso de uma falha completa em um dos datacenters, o serviço possa continuar a operar sem interrupções significativas, alternando para o datacenter emparelhado.

#### 1.3 Sovereign Regions

São regiões específicas que atendem a rigorosos requisitos governamentais e de dados.

!!! warning "Aviso"
    Regiões soberanas podem ter políticas de rede e acesso mais restritas devido às leis de proteção de dados locais.

!!! info "Exemplo"
    Microsoft Azure Government: Este é um exemplo de uma região soberana projetada especificamente para atender às necessidades do governo dos Estados Unidos, garantindo que os dados sejam armazenados e gerenciados de acordo com as regulamentações federais rigorosas.

### 2. Availability zone

Zonas de disponibilidade são datacenters separados fisicamente dentro de uma mesma região para proporcionar isolamento de falhas e redundância.

!!! tip "Dica"
    Utilize zonas de disponibilidade para construir aplicações resilientes que suportem falhas de infraestrutura sem interromper o serviço ao usuário.

#### 2.1. Como Escolher uma Availability Zone no Azure:


Primeiro, selecione a região na qual deseja implantar o recurso (por exemplo, East US 2 ou West Europe).
Seleção da Zona de Disponibilidade:

Ao configurar o recurso (como uma Máquina Virtual ou Banco de Dados), o Azure oferecerá a opção de selecionar uma zona específica, como:

- Zona 1
- Zona 2
- Zona 3
- 
Se você não selecionar uma zona específica, o Azure geralmente faz a distribuição automática do recurso entre as zonas disponíveis na região.

#### 2.2. Recursos que Permitem Escolher Availability Zones

- Máquinas Virtuais (VMs): Durante a criação, você pode optar por implantar uma VM em uma zona específica para garantir resiliência contra falhas locais.
- Discos Gerenciados (Managed Disks): Permite especificar em qual zona o disco será colocado, associado à VM.
- Balanceadores de Carga (Load Balancers): Pode ser configurado para distribuir tráfego entre recursos em diferentes zonas.
Bancos de Dados (como Azure SQL ou PostgreSQL):

Em alguns casos, você pode configurar redundância em zonas.

### 3. Datacenters do Azure

Os datacenters são instalações que abrigam servidores e outros componentes críticos, projetados para serem seguros e sustentáveis.

!!! info "Info"
    Os datacenters do Azure usam tecnologias de energia renovável e reciclagem de água, alinhando-se com as metas de sustentabilidade da Microsoft.

### 4. Recursos e Grupos de Recursos do Azure

#### 4.1 Recursos
Cada recurso no Azure é uma entidade gerenciável, como uma VM, um banco de dados SQL ou uma conta de armazenamento.

#### 4.2 Grupos de Recursos
Os grupos de recursos organizam recursos relacionados para facilitar a gestão e alocação de custos.

!!! tip "Dica"
    Organize recursos em grupos de recursos baseados em critérios como ciclo de vida, departamento ou uso para simplificar a administração e otimizar custos.

### 5. Assinaturas

Assinaturas são contêineres de cobrança e gerenciamento onde são agrupados recursos e grupos de recursos.

!!! warning "Aviso"
    Manter uma boa governança sobre as assinaturas é essencial para evitar gastos excessivos e manter a segurança.

### 6. Grupos de Gerenciamento

Grupos de gerenciamento permitem organizar assinaturas em hierarquias que refletem a estrutura organizacional.

!!! info "Info"
    Grupos de gerenciamento são ideais para aplicar políticas de governança em larga escala.

### 7. Hierarquia de Grupos de Recursos, Assinaturas e Grupos de Gerenciamento 

Esta hierarquia estruturada ajuda a organizar e gerenciar o acesso e políticas em larga escala dentro do ambiente Azure.

!!! tip "Dica"
    Utilize a hierarquia para implementar controles de acesso e políticas consistentes em todos os níveis, desde recursos individuais até grupos de gerenciamento.
