# 🔐 Identidade, Acesso e Segurança no Azure

## 🆔 Microsoft Entra ID (Azure AD)

O **Microsoft Entra ID** (anteriormente Azure Active Directory) é um serviço de **gerenciamento de identidades e acesso baseado em nuvem**. Ele oferece:

- ✅ Autenticação
- 🔑 Logon único (SSO)
- 🔗 Gerenciamento de aplicativos
- 🤝 Colaboração B2B (Business to Business)
- 📱 Gerenciamento de dispositivos

---

## 🌐 Microsoft Entra Domain Services

- Oferece serviços gerenciados equivalentes ao **Active Directory local**, como:
  - **Controladores de domínio**
  - **Sincronização de usuários e grupos**
  - **Suporte a aplicativos legados**

### 🔄 Fluxo de Sincronização:

AD Local ← (Entra Connect) → Locatário Microsoft Entra ID → Domínio Gerenciado na VNet


- Permite executar aplicativos legados e gerenciar domínio **sem a necessidade de infraestrutura de controladores de domínio locais**.

---

## 🔐 Autenticação vs Autorização

| Conceito       | Descrição                                                                 |
|----------------|---------------------------------------------------------------------------|
| **Autenticação** | Processo de **verificar a identidade** (Quem você é).                   |
| **Autorização** | Processo de **conceder permissões** (O que você pode fazer).             |

- 🔒 **Autenticação Multifator (MFA):** Adiciona uma camada extra de segurança exigindo múltiplos fatores (senha + app, biometria, etc.).

---

## 🌍 Identidades Externas no Microsoft Entra

### 🔗 **B2B - Microsoft Entra External ID**

- Permite colaboração segura com:
  - **Parceiros**
  - **Fornecedores**
  - **Outras organizações**

✅ Formas de acesso:
- **Convite**
- **Autoinscrição**

→ Usuários externos ficam registrados no **locatário Microsoft Entra ID**.

---

### 🛍️ **B2C - Azure AD B2C**

- Gerencia **identidades de consumidores** que acessam seus aplicativos.

✅ Funcionalidades:
- Fluxos de:
  - **Inscrição**
  - **Login**
- Políticas personalizadas de autenticação e autorização.

→ Gerenciado em um **locatário específico do Azure AD B2C**.

---

## 🔑 Acesso Condicional

Ferramenta para permitir ou negar acesso com base em:

- 👤 Usuário ou grupo
- 🌎 Localização (IP)
- 💻 Dispositivo
- 📱 Aplicativo
- ⚠️ Detecção de risco

✅ Aplica políticas adaptáveis de segurança.

---

## 🗝️ Controle de Acesso Baseado em Função (RBAC)

- **Gerenciamento de acesso granular** no Azure.
- Permite:
  - Dividir tarefas entre membros da equipe.
  - Conceder **apenas as permissões necessárias**.
- Aplica-se tanto ao:
  - **Portal do Azure**
  - **Recursos individuais**

---

## 🔐 Confiança Zero (Zero Trust)

### 🏛️ Abordagem Tradicional:
- Confiava em perímetros de rede internos como "seguros".

### 🚫 Abordagem Zero Trust:
- **Nunca confia automaticamente, sempre verifica.**
- Protege os ativos **onde quer que estejam**, com:
  - Políticas centralizadas
  - Verificação contínua de identidade, dispositivo e contexto

---

## 🛡️ Proteção em Camadas (Defense in Depth)

Abordagem em múltiplas camadas para mitigar riscos e isolar falhas.

### 🔒 Camadas de Segurança:

1. **Segurança Física** (Datacenters)
2. **Identidade e Acesso** (Entra ID, MFA, RBAC)
3. **Perímetro** (Firewall, Gateway)
4. **Rede** (Segmentação, NSG, VPN)
5. **Computação** (VMs, Contêineres, Patch Management)
6. **Aplicativos** (DevSecOps, WAF)
7. **Dados** (Criptografia, Gerenciamento de Chaves)

---

## 🏢 Microsoft Defender para Nuvem

- Monitoramento de:
  - 🔒 Segurança de datacenters
  - 🦠 Malware
  - 🚨 Ataques potenciais
- Funcionalidades:
  - 🔍 Recomendações de segurança
  - 🚪 Controle de acesso Just-In-Time (JIT) para portas
  - 🛡️ Detecção e bloqueio de ameaças

🔗 [Saiba mais sobre Microsoft Defender for Cloud](https://learn.microsoft.com/pt-br/azure/defender-for-cloud/)

---

## 📚 Referências Oficiais

- [Microsoft Learn - Segurança no Azure](https://learn.microsoft.com/pt-br/azure/security/)
- [Documentação do Microsoft Entra ID](https://learn.microsoft.com/pt-br/entra/)
- [Acesso Condicional no Azure](https://learn.microsoft.com/pt-br/azure/active-directory/conditional-access/)
- [Controle de Acesso RBAC no Azure](https://learn.microsoft.com/pt-br/azure/role-based-access-control/)
- [Microsoft Defender for Cloud](https://learn.microsoft.com/pt-br/azure/defender-for-cloud/)

---

## 🚀 Explore Mais

- 🌐 [Mapa da Infraestrutura Global do Azure](https://infrastructuremap.microsoft.com/)
