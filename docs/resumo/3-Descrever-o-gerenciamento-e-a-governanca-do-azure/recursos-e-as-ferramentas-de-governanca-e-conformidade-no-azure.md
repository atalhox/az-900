# Recursos e Ferramentas de Governança e Conformidade no Azure

## 1. Microsoft Purview no Azure  

O Microsoft Purview é uma ferramenta abrangente de governança de dados que ajuda as organizações a mapear, catalogar e controlar seus dados em ambientes multicloud e on-premises.  

Ele fornece uma visão unificada dos dados, permitindo gestão eficiente da informação, melhorando a privacidade de dados e garantindo a conformidade com regulamentações como GDPR e HIPAA.

### 1.1. Principais Recursos do Microsoft Purview 

- Descoberta automática de dados – Identifica, cataloga e classifica dados distribuídos em diferentes fontes.  
- Gestão de acessos – Define quem pode visualizar ou modificar determinados dados.  
- Monitoramento de conformidade – Ajuda a garantir que os dados sigam regras de compliance.  

!!! tip "Tip"
    Use o Microsoft Purview para ter controle total sobre os seus dados, garantindo segurança e conformidade em diferentes nuvens e ambientes locais.

## 2. Azure Policy  

O Azure Policy é uma ferramenta de governança automatizada que permite criar, atribuir e monitorar políticas de conformidade para os recursos do Azure.  

Essas políticas garantem que os recursos sigam normas organizacionais e regulatórias, aplicando restrições e auditorias sem intervenção manual.

### 2.1. Casos de Uso do Azure Policy  

- Restringir tipos de recursos – Exemplo: Impedir a criação de VMs fora das regiões aprovadas.  
- Aplicação de regras de segurança – Exemplo: Garantir que todas as VMs tenham discos criptografados.  
- Auditoria e conformidade – Exemplo: Detectar automaticamente configurações não conformes e gerar alertas.  

!!! info "Info"
    O Azure Policy ajuda a manter padrões de segurança e conformidade consistentes, garantindo que todos os recursos sigam as melhores práticas definidas pela organização.

## 3. Resource Locks

Os Resource Locks (Bloqueios de Recursos) são mecanismos de proteção contra alterações acidentais, evitando a exclusão ou modificação de recursos críticos.

Existem dois tipos de bloqueios no Azure:

- Bloqueio de Exclusão ("CanNotDelete") – Impede que o recurso seja excluído, mas permite modificações.  
- Bloqueio de Leitura e Escrita ("ReadOnly") – Impede qualquer modificação ou exclusão do recurso.  

### 3.1. Exemplo de Uso

- Uma empresa deseja evitar que um grupo de recursos crítico seja excluído acidentalmente. Aplicando um Resource Lock de Exclusão, qualquer tentativa de exclusão será bloqueada, garantindo segurança operacional.

!!! warning "Warning"
    Use Resource Locks em recursos essenciais como bancos de dados, firewalls e redes para evitar alterações acidentais que possam afetar serviços críticos.

## 4. Diferenças

| Solução               | Finalidade                                       | Escopo                                 | Como Funciona                                   | Exemplo de Uso                                                                | Automação | Integração Multicloud                         |
| --------------------- | ------------------------------------------------ | -------------------------------------- | ----------------------------------------------- | ----------------------------------------------------------------------------- | --------- | --------------------------------------------- |
| **Microsoft Purview** | Governança e auditoria de dados                  | Dados armazenados em múltiplas fontes  | Descobre, classifica e monitora dados sensíveis | Identificação de dados confidenciais como CPF e cartões de crédito            | Sim       | Sim – Suporta AWS, Google Cloud e On-Premises |
| **Azure Policy**      | Aplicação de conformidade e segurança            | Recursos do Azure (VMs, redes, bancos) | Aplica regras e auditorias automaticamente      | Garantir que todas as VMs estejam criptografadas e dentro da região permitida | Sim       | Não – Funciona apenas no Azure                |
| **Resource Locks**    | Proteção contra exclusão e alterações acidentais | Recursos específicos no Azure          | Bloqueia alterações e exclusões não autorizadas | Evitar que um banco de dados ou firewall seja excluído por engano             | Não       | Não – Funciona apenas no Azure                |
