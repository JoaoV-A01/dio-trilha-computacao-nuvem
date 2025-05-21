# Componentes de Arquitetura do Azure

A arquitetura do Azure é composta por vários elementos que permitem planejar, organizar e gerenciar recursos em nuvem com eficiência, escalabilidade e segurança.

---

## 🌍 Regiões do Azure

As **regiões** são áreas geográficas que contêm **um ou mais datacenters interconectados**. Elas permitem implantar recursos próximos aos usuários finais, o que reduz a latência e melhora a experiência.

- **Zonas de disponibilidade**: conjunto de datacenters independentes dentro de uma região, garantindo alta disponibilidade e redundância.
- **Residência dos dados**: conformidade com leis como a **LGPD**, que exige que certos dados não saiam do país.

🔗 [Regiões do Azure – Documentação](https://learn.microsoft.com/pt-br/azure/availability-zones/az-overview)

---

## 🌐 Pares de Regiões

- Cada região primária tem uma **região secundária emparelhada** separada por no mínimo 300 milhas (~480 km).
- Oferece **recuperação de desastres** e **replicação automática** para determinados serviços.
- Em caso de interrupções, a região emparelhada tem **prioridade de recuperação**.

🔗 [Pares de regiões do Azure](https://learn.microsoft.com/pt-br/azure/best-practices-availability-paired-regions)

---

## 🏛️ Regiões Soberanas

Algumas regiões são **isoladas geograficamente e operacionalmente** para atender a exigências específicas:

- **Azure Government (EUA)**: uso exclusivo por órgãos governamentais dos EUA. Infraestrutura separada e altamente segura.
- **Azure China**: operada pela 21Vianet, em conformidade com regulamentos locais.
  
🔗 [Azure Government](https://learn.microsoft.com/pt-br/azure/azure-government/documentation-government-welcome)  
🔗 [Azure China](https://learn.microsoft.com/en-us/azure/china/overview)

---

## ⚙️ Recursos do Azure

São os **blocos de construção** usados para criar soluções na nuvem:

- Máquinas Virtuais (VMs)
- Contas de Armazenamento
- Redes Virtuais
- Bancos de Dados SQL
- Azure Functions
- Azure App Services

🔗 [Tipos de recursos no Azure](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/azure-services-resource-manager)

---

## 🧱 Grupos de Recursos

- Funcionam como **containers lógicos** para agrupar e gerenciar recursos relacionados de um projeto.
- Exemplo: um grupo para recursos de front-end, outro para banco de dados.
- Recursos podem:
  - Ser movidos entre grupos.
  - Pertencer a grupos diferentes dentro da mesma aplicação.

🔗 [Gerenciar grupos de recursos](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/manage-resource-groups-portal)

---

## 💳 Assinaturas do Azure

- Cada assinatura representa uma **unidade de cobrança** e **controle de acesso**.
- Um projeto pode ter diferentes assinaturas para ambientes distintos, como:
  - Desenvolvimento
  - Teste
  - Produção

### Benefícios:
- **Limite de cobrança**: separa relatórios e faturas por assinatura.
- **Controle de acesso**: define permissões por assinatura.

---

## 🗂️ Grupos de Gerenciamento

- Usados para **organizar e aplicar políticas** sobre várias assinaturas.
- Facilitam o gerenciamento de múltiplos projetos e equipes em uma empresa.

🔗 [Gerenciar vários assinaturas com grupos de gerenciamento](https://learn.microsoft.com/pt-br/azure/governance/management-groups/overview)

---

## 🧪 Lab: Construindo Arquiteturas no Azure

💡 A Microsoft oferece um site interativo com uma **visualização imersiva da infraestrutura global** do Azure, incluindo:

- Mapa de regiões e zonas.
- Visualização dos datacenters.
- Chatbot com informações sobre cada área.

🔗 [Explore | Azure Global Infrastructure Experience](https://infrastructuremap.microsoft.com)

### Criando Grupos de Recursos

1. Selecione a **assinatura**.
2. Defina o **nome do grupo** e a **região**.
3. (Opcional) Aplique **marcas (tags)** com chave-valor para organização lógica (ex: `ambiente=produção`).
4. Faça a revisão e conclua a criação.

🔗 [Criar e gerenciar grupos de recursos – Portal Azure](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/manage-resource-groups-portal)

### Ferramentas Disponíveis em Grupos de Recursos

- **IAM (Controle de Acesso)**
- **Logs de Atividade**
- **Implantações**
- **Segurança**
- **Criação de novos recursos (como redes virtuais, bancos de dados, etc.)**

---
