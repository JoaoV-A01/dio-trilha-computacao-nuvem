# ☁️ Computação e Rede no Azure

## 🚀 Serviços de Computação do Azure

A computação no Azure é um serviço sob demanda que fornece recursos como:

- Processamento (CPU)
- Memória
- Disco
- Rede
- Sistema operacional

### Exemplos de Serviços de Computação:

- **Máquinas Virtuais (VMs)**
- **App Service (Aplicativos de Serviços)**
- **Contêineres e Instâncias de Contêiner**
- **Azure Kubernetes Service (AKS)**
- **Azure Virtual Desktop (Área de Trabalho Virtual)**
- **Azure Functions (Serverless)**

---

## 💻 Máquinas Virtuais do Azure (VM)

- São **emulações de computadores físicos**, incluindo processador, memória, disco e rede.
- Fazem parte do modelo **IaaS (Infraestrutura como Serviço)**, oferecendo **personalização total**, mas com maior responsabilidade sobre configuração, segurança e atualizações.

🔗 [Documentação de VMs no Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/)

### 🔄 Conjuntos de Dimensionamento de VMs

- Permitem escalar automaticamente conforme a demanda.
- Oferecem **balanceamento de carga** e alta disponibilidade.

### 🏢 Conjuntos de Disponibilidade de VMs

- Distribuem as VMs em **racks físicos diferentes** dentro dos datacenters.
- Garantem continuidade em caso de **falhas ou manutenções programadas**.

---

## 🖥️ Azure Virtual Desktop (Área de Trabalho Virtual)

- Virtualização de **área de trabalho e aplicativos** diretamente na nuvem.
- Suporte a **múltiplas sessões simultâneas** no mesmo ambiente.
- Reduz riscos de perda de dados e facilita acessos remotos.

🔗 [Documentação do Azure Virtual Desktop](https://learn.microsoft.com/pt-br/azure/virtual-desktop/)

---

## 📦 Serviços de Contêineres no Azure

- Ambiente virtualizado, **leve e isolado**, sem necessidade de gerenciar sistemas operacionais.

### 🔹 Instâncias de Contêiner (ACI)

- Modelo **PaaS**, executa um contêiner isolado rapidamente, sem orquestração.

### 🔸 Azure Container Apps

- **PaaS** com recursos como **escalonamento automático** e **balanceamento de carga**.

### 🚢 Azure Kubernetes Service (AKS)

- Serviço de **orquestração de contêineres** baseado no Kubernetes.
- Ideal para arquiteturas distribuídas e cargas de trabalho complexas.

---

## ⚡ Azure Functions (Serverless)

- Executa **funções baseadas em eventos** sem gerenciar servidores.
- **Paga-se apenas pelo tempo de execução**.
- Ideal para automações, processamento em segundo plano e APIs leves.

🔗 [Documentação do Azure Functions](https://learn.microsoft.com/pt-br/azure/azure-functions/)

---

## 📊 Comparação de Opções de Computação

| Opção               | Descrição                                                                                   | Modelo   |
|---------------------|----------------------------------------------------------------------------------------------|----------|
| **Máquinas Virtuais** | Servidores completos para Windows e Linux. Suporte a lift-and-shift.                      | IaaS     |
| **Área de Trabalho Virtual** | Ambientes de desktop virtualizados com múltiplos logins simultâneos.                   | SaaS     |
| **Contêineres**       | Microsserviços empacotados em ambientes leves e isolados.                                 | PaaS     |
| **App Service**       | Plataforma gerenciada para desenvolvimento e hospedagem de aplicativos web e APIs.        | PaaS     |
| **Azure Functions**   | Computação sem servidor, baseada em eventos.                                               | FaaS     |

---

## 🌐 Serviços de Rede do Azure

A **Rede Virtual (VNet)** permite a comunicação entre recursos no Azure, na internet e em redes locais.

### 🔗 Principais Serviços de Rede:

- **VNet**: Rede privada no Azure.
- **Sub-redes**: Segmentam a VNet.
- **Emparelhamento de Rede**: Conecta VNets em diferentes regiões.

### 🔒 Gateway de VPN

- Cria uma conexão **criptografada** entre a rede local e o Azure pela internet pública.

### ⚡ ExpressRoute

- Conexão privada, mais rápida e segura, entre redes locais e o Azure (sem passar pela internet).

### 🌐 DNS do Azure

- Serviço de resolução de nomes DNS altamente disponível e seguro.
- Usa infraestrutura global com tecnologia **Anycast**.

🔗 [Documentação sobre Rede no Azure](https://learn.microsoft.com/pt-br/azure/networking/)

---

## 🔧 Lab: Configurando Recursos e Dimensionamento de VMs

### 🖥️ Criação de Máquinas Virtuais

- Escolha entre **modelos prontos** ou configuração manual.
- Etapas principais:
  - Tipo de assinatura
  - Nome e região
  - Opções de disponibilidade
  - Conjuntos de dimensionamento
  - Tipo de segurança e imagem
  - Arquitetura da VM (geração e tamanho)
  - Regras de portas de entrada (Firewall)
  - Configuração de Spot Instance (economia com disponibilidade não garantida)

### 💽 Configuração de Disco

- Definir tipo (Standard, Premium ou Ultra).
- Vincular a exclusão do disco à exclusão da VM.
- Gerenciamento de chaves e discos existentes.

### 🌐 Configuração de Rede

- Sub-rede
- IP público ou privado
- Rede acelerada
- Controle de NAT e firewall

### 🔧 Gerenciamento e Monitoramento

- Desligamento automático
- Backup
- Atualizações do sistema operacional convidado
- Monitoramento de integridade e logs
- Alertas e diagnósticos

### 🔑 Avançado

- Extensões
- Dados personalizados
- Reservas de capacidade
- Aplicação de tags (chave-valor)

---

## 🖥️ Criação de Área de Trabalho Virtual

- Definir o tipo de **pool de hosts**:
  - **Compartilhado:** para múltiplos usuários.
  - **Dedicado:** para um usuário ou aplicação específica.
- Informar:
  - Assinatura
  - Nome
  - Região
  - Ambiente de validação (produção ou teste)

---

## ⚡ Criação de Azure Functions

- Configuração:
  - Nome
  - Região
  - Versão e pilha de runtime (.NET, Node.js, Python, Java, etc.)
  - Tipo de hospedagem (consumo ou dedicado)
- Outras opções:
  - Armazenamento
  - Rede
  - Monitoramento
  - Rótulos (tags)
- Finalizar com **revisão e criação**.

---

## 🔍 Referências Oficiais

- [Microsoft Learn - Azure](https://learn.microsoft.com/pt-br/azure/)
- [Documentação de VMs](https://learn.microsoft.com/pt-br/azure/virtual-machines/)
- [Documentação de Redes no Azure](https://learn.microsoft.com/pt-br/azure/networking/)
- [Documentação de Azure Functions](https://learn.microsoft.com/pt-br/azure/azure-functions/)
- [Documentação de App Service](https://learn.microsoft.com/pt-br/azure/app-service/)

---

## 🚀 Explore mais

- 🌐 [Mapa da Infraestrutura Global do Azure](https://infrastructuremap.microsoft.com/)
