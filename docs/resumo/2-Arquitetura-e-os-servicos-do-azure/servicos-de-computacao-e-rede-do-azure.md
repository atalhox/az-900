# Azure Compute e Networking Services

## 1. Comparação de Tipos de Computação

### 1.1. **Contêineres**

Permitem que os desenvolvedores empacotem aplicações com todas as suas dependências em contêineres isolados. São ideais para aplicações que requerem consistência entre ambientes de desenvolvimento, teste e produção.

### 1.2. **Máquinas Virtuais (VMs)**

Oferecem um ambiente de computação virtualizado completo para executar sistemas operacionais e aplicações. São adequadas para aplicações que necessitam de acesso completo ao sistema operacional e recursos dedicados.

### 1.3.  **Funções (Azure Functions)**

São parte da oferta de computação sem servidor do Azure, permitindo que os desenvolvedores executem pequenos blocos de código em resposta a eventos, sem preocupar-se com a infraestrutura subjacente.

!!! tip "Dica"
    Escolha **Contêineres** para portabilidade, **VMs** para controle total sobre o ambiente e **Azure Functions** para execução de código sob demanda sem gerenciar servidores.

## 2. Opções de Máquina Virtual

- **Máquinas Virtuais do Azure**: Oferecem computação em nuvem escalável com uma variedade de opções de configuração, incluindo diferentes CPUs, memórias e capacidades de armazenamento.

- **Conjuntos de Dimensionamento de Máquinas Virtuais do Azure**: Permitem que as VMs sejam escaladas para cima ou para baixo automaticamente com base em métricas de desempenho, facilitando o gerenciamento de picos de demanda.

- **Conjuntos de Disponibilidade**: Agrupam VMs de modo que as falhas de hardware ou de rede afetem apenas uma pequena parte das VMs, aumentando a disponibilidade geral da aplicação.

- **Área de Trabalho Virtual do Azure**: Proporciona uma solução de desktop virtualizada, permitindo que os usuários acessem um ambiente de desktop completo e seguro de qualquer dispositivo.

!!! info "Info"
    O **Conjunto de Dimensionamento de VMs** é ideal para aplicações que precisam crescer dinamicamente, enquanto os **Conjuntos de Disponibilidade** aumentam a resiliência contra falhas.

## 3. Recursos Necessários para Máquinas Virtuais

- **CPU, Memória e Armazenamento**: Recursos essenciais que definem o desempenho da VM.
- **Rede e Conectividade**: Inclui configurações de IP, balanceamento de carga e firewalls.
- **Sistema Operacional**: Imagens de sistemas operacionais disponíveis, como Windows ou Linux.
- **Disco de Backup e Recuperação**: Opções para proteção e recuperação de dados.

!!! warning "Aviso"
    Sempre configure **discos gerenciados** e backup para proteger dados críticos, evitando perda de informações caso ocorra uma falha.

## 4. Opções de Hospedagem de Aplicativos

- **Aplicativos Web (Azure App Service)**: Permite o desenvolvimento e hospedagem de aplicativos web e APIs em um ambiente gerenciado, com autoescalabilidade e integração de alto nível.

- **Contêineres (Azure Kubernetes Service, AKS)**: Oferece um ambiente de orquestração de contêineres para gerenciar e escalar aplicações contêinerizadas de maneira eficiente.

- **Máquinas Virtuais**: Apropriadas para aplicações que necessitam de configurações específicas do servidor ou que não são adequadas para execução em plataformas de alto nível.

!!! tip "Dica"
    **Azure App Service** é ideal para aplicações web padrão, enquanto o **Azure Kubernetes Service (AKS)** é recomendado para workloads baseados em contêineres que exigem escalabilidade.

## 5. Rede Virtual

- **Azure Virtual Network (VNet)**: Permitem que muitos tipos de recursos do Azure, como VMs, se comuniquem de forma segura, isolada e escalável.

- **Azure Virtual Subnets**: Segmentam uma VNet em múltiplas redes isoladas que podem ser gerenciadas e seguradas separadamente.

- **VNet Peering**: Conecta duas VNets, permitindo que elas se comuniquem como se estivessem na mesma rede.

- **Azure DNS**: Fornece hospedagem de DNS e resolução de nomes dentro das VNets.

- **Azure VPN Gateway**: Conecta redes locais à VNet do Azure através de uma conexão de VPN segura.

- **Azure ExpressRoute**: Permite uma conexão privada entre a infraestrutura local e o Azure, sem passar pela internet pública.

!!! info "Info"
    **ExpressRoute** fornece maior segurança e desempenho que VPNs tradicionais, tornando-o a melhor escolha para conexões corporativas de alto desempenho.

## 6. Pontos de Extremidade Públicos e Privados

### 6.1. Public Endpoints

Public Endpoints são acessíveis pela internet e permitem que serviços do Azure sejam consumidos globalmente.

#### 6.1.1. Azure Storage Account (Public Access)
Se você configurar uma **Azure Storage Account** com um **Public Endpoint**, qualquer usuário com o link pode acessar os arquivos armazenados nela, a menos que restrições de acesso sejam aplicadas.

#### 6.1.2 Azure Web App (Public Access)
Um **Azure App Service (Web App)** pode ser configurado com um **Public Endpoint**, tornando-o acessível globalmente através de um domínio público, como `mywebapp.azurewebsites.net`.

#### 6.1.3. Azure SQL Database (Public Access)
Se um banco de dados SQL no Azure for configurado para permitir conexões de **qualquer IP**, ele estará acessível publicamente, podendo ser acessado por aplicativos em qualquer parte do mundo.

!!! warning "Atenção"
    Expor recursos com **Public Endpoints** pode ser um risco de segurança se não houver controle adequado, como firewalls, regras de rede ou autenticação reforçada.

### 6.2. Private Endpoints 

Private Endpoints fornecem conexões privadas dentro de uma **Azure Virtual Network (VNet)**, garantindo que o tráfego de dados nunca saia da rede do Azure ou seja exposto na internet pública.

#### 6.2.1. Azure Storage Account (Private Endpoint)
Configurar um **Private Endpoint** para uma **Azure Storage Account** permite que apenas máquinas dentro da **VNet** tenham acesso ao armazenamento, bloqueando completamente acessos externos.

#### 6.2.2. Azure SQL Database (Private Endpoint)

Um **Azure SQL Database** pode ser acessado apenas por servidores ou aplicações dentro de uma **VNet** específica, eliminando a necessidade de expor o banco à internet.

#### 6.2.3. Azure Kubernetes Service (AKS) with Private Endpoint

Um **Azure Kubernetes Service (AKS)** pode ser configurado para utilizar **Private Endpoints**, garantindo que o tráfego entre seus contêineres e outros serviços do Azure permaneça interno e seguro.

!!! tip "Dica"
    Utilize **Private Endpoints** para aumentar a segurança dos seus serviços, evitando exposição desnecessária à internet e garantindo conformidade com políticas internas de segurança.
