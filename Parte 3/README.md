# Tipos de Serviço de Nuvem

A computação em nuvem oferece diferentes modelos de serviço para atender às diversas necessidades de usuários e empresas. Os principais são:

---

## IaaS (Infrastructure as a Service)

- Fornece infraestrutura de TI como serviço: servidores, armazenamento, redes e sistemas operacionais.
- Permite **personalizar** os recursos e **pagar somente pelo que for utilizado**.
- Aplica-se tanto a ambientes locais (on-premises) quanto à nuvem.
- Ideal para empresas que precisam de controle sobre sua infraestrutura sem arcar com os custos de manter hardware físico.

🔗 [O que é IaaS - Microsoft Learn](https://learn.microsoft.com/pt-br/azure/architecture/cloud-adoption/getting-started/iaas)

---

## PaaS (Platform as a Service)

- Constrói sobre o IaaS, fornecendo também ferramentas de desenvolvimento, banco de dados, análise e gerenciamento.
- Permite que desenvolvedores **fiquem focados no desenvolvimento e implantação de aplicações**, sem se preocupar com a manutenção da infraestrutura subjacente.
- Facilita o desenvolvimento ágil e a automação do ciclo de vida das aplicações.

🔗 [O que é PaaS - Microsoft Learn](https://learn.microsoft.com/pt-br/azure/architecture/cloud-adoption/getting-started/paas)

---

## SaaS (Software as a Service)

- Fornece software pronto para uso que é gerenciado inteiramente pelo provedor.
- Os usuários acessam os aplicativos via internet, com foco apenas em sua utilização.
- Exemplo: Microsoft Teams, Microsoft 365, Outlook, OneDrive, entre outros.

🔗 [O que é SaaS - Microsoft Learn](https://learn.microsoft.com/pt-br/azure/architecture/cloud-adoption/getting-started/saas)

---

## Modelo de Responsabilidade Compartilhada

Na computação em nuvem, as responsabilidades são divididas entre o **cliente** e o **provedor de nuvem**, dependendo do tipo de serviço contratado.

📌 No modelo **on-premises**, toda a responsabilidade é do cliente.

📌 Na nuvem, algumas camadas são gerenciadas pelo provedor, outras continuam sob responsabilidade do cliente — como **dados, identidades e dispositivos**.

🔗 [Modelo de responsabilidade compartilhada no Azure](https://learn.microsoft.com/pt-br/azure/security/fundamentals/shared-responsibility)

### Exemplo de Distribuição de Responsabilidades

| Item                        | SaaS         | PaaS         | IaaS         |
|----------------------------|--------------|--------------|--------------|
| Infraestrutura e datacenter | Microsoft    | Microsoft    | Microsoft    |
| Sistema operacional         | Microsoft    | Microsoft    | Cliente      |
| Controles de rede           | Microsoft    | Compartilhada| Cliente      |
| Aplicações                  | Microsoft    | Compartilhada| Cliente      |
| Identidade e diretórios     | Compartilhada| Compartilhada| Cliente      |
| Dados, dispositivos e contas| Cliente      | Cliente      | Cliente      |

---

## Lab: Configurando uma Instância de Banco de Dados no Azure

### 1. Criando uma Máquina Virtual
- É possível configurar o sistema operacional, discos, regras de rede, gerenciamento, monitoramento, entre outros.
- Todo esse ambiente será de **responsabilidade do cliente**, portanto é essencial um planejamento cuidadoso.

🔗 [Criar uma máquina virtual Linux no Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/linux/quick-create-portal)  
🔗 [Criar uma máquina virtual Windows no Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)

### 2. Criando um Servidor de Banco de Dados SQL
- Durante a configuração, é possível escolher localização geográfica, redundância, desempenho e regras de segurança.
- A **calculadora de preços** integrada ao portal estima os custos com base nas escolhas feitas.

🔗 [Criar instância SQL no Azure](https://learn.microsoft.com/pt-br/azure/azure-sql/database/single-database-get-started-portal)

---

## Ferramenta útil

🧮 [Calculadora de Preços do Azure](https://azure.microsoft.com/pt-br/pricing/calculator/): planeje os custos com base na configuração de máquinas, bancos de dados, redes e mais.

---
