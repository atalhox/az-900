# Identidade, Acesso e Segurança no Azure

## 1. Serviços de Diretório no Azure

### 1.1. Microsoft Entra ID (anteriormente Azure Active Directory ou Azure AD)

É o serviço de diretório baseado em nuvem da Microsoft. 

Ele oferece um conjunto abrangente de funcionalidades de gerenciamento de identidade e acesso, incluindo gerenciamento de usuários, grupos, e aplicativos, com integração com diretórios locais e suporte a padrões de identidade como SAML e OAuth.

### 1.2. Microsoft Entra Domain Services

Este serviço do Azure facilita a migração de sistemas que dependem do Active Directory (AD) tradicional para a nuvem. 

O Active Directory é como uma lista telefônica corporativa que gerencia as credenciais e os direitos dos usuários, permitindo-lhes acessar recursos de TI específicos dentro de uma organização. 

O Microsoft Entra Domain Services permite que você leve essas funcionalidades para a nuvem sem ter que modificar seus aplicativos existentes. 

Isso elimina a necessidade de reconfigurar ou reprogramar seus aplicativos para trabalhar com um novo sistema de autenticação na nuvem.

!!! tip "Dica para Serviços de Diretório"
    Aproveite os serviços de diretório no Azure para centralizar o gerenciamento de identidades e melhorar a segurança, facilitando a administração e o acesso aos recursos em escala.

## 2. Métodos de Autenticação no Azure

### 2.1. SSO (Logon Único)

Permite que os usuários acessem múltiplos serviços e aplicações com um único conjunto de credenciais, melhorando a experiência do usuário e a segurança.

### 2.2. MFA (Autenticação Multifator)

Adiciona uma camada de segurança exigindo dois ou mais métodos de verificação da identidade do usuário antes de conceder acesso.

### 2.3. Acesso sem senha

Utiliza métodos como biometria, tokens ou aplicativos de autenticação para eliminar a necessidade de senhas, reduzindo o risco de ataques baseados em roubo de senhas.

!!! tip "Dica para Métodos de Autenticação"
    Implementar MFA e acesso sem senha para reforçar a segurança, especialmente para acessos críticos e informações sensíveis.

## 3. Identidades Externas no Azure

### 3.1. B2B (Business-to-Business)

Permite que organizações colaborem de forma segura com parceiros externos, concedendo acesso a recursos específicos do Azure sem criar contas de usuário completas.

!!! tip "Dica para B2B"
    Utilize o B2B para facilitar a colaboração segura com parceiros sem a necessidade de integrar totalmente seus sistemas de TI, garantindo assim que ambas as partes mantenham controle e segurança sobre seus dados.

### 3.2. B2C (Business-to-Customer)

É uma solução de gerenciamento de identidades para aplicações voltadas ao consumidor que permite personalizar e controlar como os clientes se inscrevem, entram e gerenciam seus perfis.

!!! tip "Dica para B2C"
    Implemente o B2C para oferecer uma experiência de usuário personalizada e segura em suas aplicações voltadas ao consumidor, aprimorando o engajamento e a satisfação do cliente.

### 4. Acesso Condicional do Microsoft Entra

Permite definir políticas que ajustam o acesso aos recursos com base no contexto da solicitação de acesso, como localização do usuário, dispositivo utilizado, e riscos de segurança detectados, garantindo que apenas solicitações de acesso confiáveis sejam atendidas.

!!! tip "Dica para Acesso Condicional"
    Aproveite o acesso condicional para reforçar a segurança, especialmente em ambientes de trabalho flexíveis, garantindo que o acesso seja concedido de forma inteligente e situacional.

### 5. RBAC (Controle de Acesso Baseado em Função) do Azure

Define permissões com base em funções dentro do Azure, garantindo que os usuários tenham apenas o acesso necessário para desempenhar suas funções específicas. Isso minimiza riscos de segurança e simplifica a gestão de permissões.

!!! tip "Dica para RBAC"
    Use o RBAC para minimizar os riscos de segurança, atribuindo aos usuários apenas as permissões necessárias para suas funções, evitando excessos que poderiam levar a brechas de segurança.

### 6. Conceito de Zero Trust

Baseia-se no princípio de "nunca confiar, sempre verificar". Este modelo de segurança assume que ameaças podem existir tanto dentro quanto fora da rede corporativa, e que cada tentativa de acesso a recursos deve ser verificada para garantir que seja legítima.

!!! tip "Dica para Confiança Zero"
    Implemente a Confiança Zero em sua organização para maximizar a segurança, assumindo que todas as solicitações de acesso internas e externas podem ser uma potencial ameaça e devem ser verificadas rigorosamente.

### 7. Finalidade do Modelo Defense in Depth

Este modelo utiliza múltiplas camadas de segurança para proteger os recursos de TI, incluindo a segurança física, a segurança de rede, a segurança do aplicativo, a segurança dos dados, e políticas e procedimentos, tornando mais difícil para um ataque ser bem-sucedido.

!!! tip "Dica para Defesa em Profundidade"
    Adote um modelo de Defesa em Profundidade para criar múltiplas barreiras contra ataques, garantindo que, mesmo se uma camada falhar, outras ainda estarão em vigor para proteger seus recursos.

### 8. Finalidade do Microsoft Defender para Nuvem

Anteriormente conhecido como Azure Security Center, o Microsoft Defender para Nuvem oferece ferramentas integradas de segurança que ajudam a proteger os recursos do Azure e de outros ambientes de nuvem. 

Ele monitora e protege contra ameaças, gerencia a postura de segurança e oferece defesa contra ataques.

!!! tip "Dica para Microsoft Defender para Nuvem"
    Utilize o Microsoft Defender para Nuvem para uma visão abrangente e gerenciamento contínuo da segurança dos seus recursos em nuvem, melhorando a detecção de ameaças e a resposta a incidentes.