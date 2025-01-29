# Azure Storage Services

## 1. Azure Blob Storage

### Descrição
O Azure Blob Storage é um serviço para armazenar grandes quantidades de dados não estruturados, como textos ou dados binários, que podem ser acessados de qualquer lugar do mundo via HTTP ou HTTPS. 

É ideal para armazenar arquivos como imagens, vídeos, dados de áudio ou backups de grandes volumes.

!!! tip "Tip"
    Use Azure Blob Storage para armazenar backups, logs e arquivos estáticos usados por aplicativos web e móveis.


## 2. Azure File Storage

### Descrição
O Azure File Storage oferece serviços de armazenamento de arquivos gerenciados que podem ser acessados simultaneamente por máquinas virtuais e aplicações locais usando o protocolo SMB (Server Message Block). 

É útil para cenários de migração de dados corporativos, compartilhamento de arquivos e persistência de dados para aplicações legadas que utilizam compartilhamento de arquivos.

!!! info "Info"
    Diferente do Blob Storage, o Azure File Storage permite acesso simultâneo a arquivos estruturados como uma unidade de rede mapeada.

## 3. Azure Queue Storage

O Azure Queue Storage é um serviço de mensageria que permite a comunicação assíncrona entre diferentes partes de um sistema distribuído. 

Ele armazena mensagens em formato de fila (FIFO - First In, First Out), permitindo que diferentes componentes de uma aplicação se comuniquem sem depender da disponibilidade imediata um do outro.

Isso é útil para desacoplar serviços, garantindo que as mensagens sejam entregues de maneira confiável, mesmo se um dos componentes estiver temporariamente indisponível.

### 3.1. Exemplo Prático
Imagine um e-commerce que processa pedidos. 

Quando um cliente finaliza uma compra, o pedido pode ser colocado na fila do Azure Queue Storage, e outro serviço, responsável pelo processamento do pagamento e envio do pedido, pode ler as mensagens dessa fila e executá-las conforme os recursos estiverem disponíveis.

Dessa forma:

- O pedido é registrado e colocado na fila, sem precisar aguardar o processamento imediato.
- O serviço de pagamento consome a mensagem da fila e processa o pagamento.
- Outro serviço consome a mensagem e agenda o envio do pedido ao cliente.

Essa abordagem melhora a escalabilidade e evita que falhas temporárias causem perda de informações.

!!! tip "Dica" 
    Use Queue Storage para gerenciar cargas de trabalho assíncronas, garantindo que as tarefas sejam processadas independentemente da disponibilidade imediata dos serviços envolvidos.

## 4. Azure Table Storage

O Azure Table Storage é um serviço que armazena grandes quantidades de dados estruturados. O serviço é NoSQL e oferece capacidade de armazenar dados menos complexos que não requerem esquemas relacionais completos, sendo ideal para armazenar tabelas grandes de informações não relacionais.

!!! warning "Warning"
    Azure Table Storage é uma solução NoSQL básica; se precisar de consultas mais avançadas ou integração com outras ferramentas analíticas, considere o Azure Cosmos DB.

## 5. Azure Disk Storage

O Azure Disk Storage fornece discos gerenciados para máquinas virtuais do Azure, serviços como Azure Kubernetes Service (AKS), e qualquer serviço que requeira armazenamento de disco persistente. 

Oferece vários tipos de discos, como SSDs (Solid State Drives) para alto desempenho e HDDs (Hard Disk Drives) para cenários menos críticos, garantindo a persistência e segurança dos dados.

!!! tip "Tip"
    Escolha Premium SSDs para aplicações de alta performance e Standard HDDs para workloads com menor demanda de IOPS.

## 6. Azure Data Lake Storage

O Azure Data Lake Storage é uma solução de armazenamento de dados altamente escalável e segura para big data analytics.

Ele combina a escalabilidade e economia do armazenamento de objetos com a confiabilidade e desempenho do armazenamento de arquivos, otimizado para análise de grandes volumes de dados.

!!! info "Info"
    Azure Data Lake Storage é otimizado para grandes volumes de dados e integra-se com ferramentas como Azure Synapse Analytics e Databricks.
