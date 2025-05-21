# Componentes de Arquitetura do Azure

## 🌍 Regiões

O Azure possui **vários datacenters distribuídos globalmente**, permitindo a utilização de recursos em diversas regiões. Isso reduz a **latência** e melhora o tempo de resposta dos serviços.

- As **regiões** geralmente são compostas por **um ou mais datacenters próximos**, formando **zonas de disponibilidade**, com pelo menos um datacenter reserva.
- As regiões oferecem **flexibilidade, escala e conformidade**, como exigências de **residência de dados** (ex: LGPD no Brasil impede que certas informações saiam do país).

### 🔄 Pares de Regiões

- Cada região principal tem uma **região secundária emparelhada** para **recuperação de desastres**.
- Pares são separados por no mínimo **300 milhas** (~480 km).
- Alguns serviços realizam **replicação automática** entre regiões.
- A recuperação das regiões emparelhadas é **priorizada em caso de interrupções**.

### 🏛️ Regiões Soberanas

- **Azure Government (EUA):** Isolado fisicamente, voltado para agências federais e estaduais.
- **Azure China:** Operado pela 21Vianet, atende à regulamentação local. A Microsoft é o primeiro provedor estrangeiro de nuvem pública na China.

---

## 🧩 Recursos do Azure

São os **componentes fundamentais** utilizados para construir soluções em nuvem:

- **Máquinas Virtuais (VMs)**
- **Contas de Armazenamento**
- **Redes Virtuais**
- **Bancos de Dados SQL**
- **Funções (Functions)**
- **Serviços de Aplicativos (App Services)**

---

## 📦 Grupos de Recursos

Forma de **organizar e gerenciar recursos relacionados** de um projeto, como um contêiner lógico.

- Exemplo: Grupo para **Web + Banco**, Grupo de **VMs**, Grupo de **Armazenamento**.
- **Recursos podem ser movidos** entre diferentes grupos.
- **Aplicativos podem usar recursos de múltiplos grupos**.

---

## 💳 Assinaturas do Azure

Cada **assinatura** está ligada a uma conta de cobrança. É possível separar projetos em diferentes assinaturas, como:

- Desenvolvimento
- Testes
- Produção

### Vantagens:

- **Limite de cobrança:** Relatórios e faturas separados por assinatura.
- **Limite de controle de acesso:** Gerenciamento de quem pode provisionar e acessar recursos.
- **Grupos de gerenciamento:** Agrupam e aplicam políticas a múltiplas assinaturas.

---

## 🧪 Lab: Construindo Arquiteturas no Azure

O Azure oferece um [site interativo da infraestrutura global](https://infrastructuremap.microsoft.com/), com:

- Visualização das regiões e pares de regiões
- Detalhes sobre replicação de dados
- Simulação de datacenters (salas, equipamentos)
- Chatbot para dúvidas

### ✅ Criando Grupos de Recursos

1. **Definir assinatura**, nome e região.
2. (Opcional) **Aplicar marcações** com chave-valor para organizar os recursos logicamente.
3. **Revisar e criar**.

Após a criação, é possível:

- Acessar logs de atividade
- Gerenciar acesso via **IAM**
- Visualizar implantações e configurações de segurança
- Criar recursos como **redes virtuais** e incluir dentro de um grupo especifico

---
