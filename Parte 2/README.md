# Benefícios da Computação em Nuvem

## Alta Disponibilidade

- Os recursos estão disponíveis sempre que o usuário precisa acessá-los.
- **SLA (Service Level Agreement)** define o nível de disponibilidade garantido por serviço (ex: 99%, 99,99%).
- Se o SLA não for cumprido, a provedora é responsável por corrigir o problema e oferecer crédito proporcional ao tempo de indisponibilidade.

🔗 [Documentação oficial de SLA do Azure](https://learn.microsoft.com/pt-br/azure/architecture/framework/resiliency/service-level-agreements)

## Escalabilidade

- Capacidade de ajustar recursos com base na demanda.
- Recursos podem ser aumentados para lidar com picos de uso e reduzidos quando a demanda diminui.
- Os custos variam conforme o uso, otimizando o investimento.

🔗 [Como escalar serviços no Azure](https://learn.microsoft.com/pt-br/azure/architecture/best-practices/auto-scaling)

## Elasticidade

- Ajuste automático ou manual de recursos em resposta a aumentos ou reduções abruptas na demanda.
- Possibilidade de adicionar/remover máquinas virtuais ou containers rapidamente.

🔗 [Documentação sobre elasticidade no Azure](https://learn.microsoft.com/pt-br/azure/architecture/patterns/elastic-scale)

## Confiabilidade

- A infraestrutura de nuvem é naturalmente confiável e resiliente devido ao seu design descentralizado.
- Recursos podem ser implementados em diferentes regiões do mundo, garantindo continuidade mesmo em falhas locais.

🔗 [Regiões do Azure e alta disponibilidade](https://azure.microsoft.com/pt-br/explore/global-infrastructure/geographies/)

## Previsibilidade

- Os serviços de nuvem oferecem controle detalhado sobre os recursos, o que facilita a previsão de custos e desempenho.
- Isso proporciona maior confiança e planejamento por parte dos usuários.

🔗 [Calculadora de preços do Azure](https://azure.microsoft.com/pt-br/pricing/calculator/)

## Segurança

- A nuvem oferece diversas ferramentas e serviços voltados à segurança.
- A responsabilidade é compartilhada: o provedor oferece a infraestrutura segura, mas a configuração e boa parte das proteções devem ser feitas pelo cliente.

🔗 [Responsabilidade compartilhada na segurança do Azure](https://learn.microsoft.com/pt-br/azure/security/fundamentals/shared-responsibility)

## Governança

- Mecanismos de auditoria permitem rastrear e sinalizar o uso de recursos.
- Permite gerenciamento específico por recurso, região ou aplicação, assegurando controle e conformidade.

🔗 [Visão geral de governança na nuvem](https://learn.microsoft.com/pt-br/azure/governance/)

## Gerenciabilidade

- O Azure oferece várias ferramentas para gerenciar os recursos:
  - Escalonamento automático com base na demanda.
  - Implantação de recursos com modelos pré-configurados.
  - Gerenciamento por meio do portal, APIs, PowerShell, CLI, entre outros.

🔗 [Gerenciamento de recursos com Azure Resource Manager](https://learn.microsoft.com/pt-br/azure/azure-resource-manager/management/overview)

---

## Lab: Criando Máquinas Virtuais no Azure

Durante o laboratório, é possível experimentar a criação de máquinas virtuais utilizando o Azure Portal. O processo permite:

- Escolher a imagem do sistema operacional.
- Configurar tamanho e recursos.
- Definir regras de rede e segurança.
- Avaliar escalabilidade e gerenciamento via portal.

🔗 [Tutorial: Criar uma máquina virtual Linux no Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/linux/quick-create-portal)

🔗 [Tutorial: Criar uma máquina virtual Windows no Azure](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)

---

## SLA (Service Level Agreement) e Tempo de Inatividade

| Nível de SLA | Inatividade semanal | Inatividade mensal | Inatividade anual  |
|--------------|---------------------|---------------------|---------------------|
| 99%          | 1,68 horas          | 7,2 horas           | 3,65 dias           |
| 99,5%        | 50,4 minutos        | 3,6 horas           | 1,83 dias           |
| 99,9%        | 10,1 minutos        | 43,2 minutos        | 8,76 horas          |
| 99,99%       | 1,01 minuto         | 4,32 minutos        | 52,56 minutos       |
| 99,999%      | 6 segundos          | 25,9 segundos       | 5,26 minutos        |

> ⚠️ Com base no contexto do projeto, é importante analisar qual o nível de **tolerância à indisponibilidade** dos recursos.

- No armazenamento, **redundância** significa que os dados são replicados em várias regiões, aumentando a confiabilidade e impactando diretamente o SLA.

🔗 [Redundância e alta disponibilidade no Armazenamento do Azure](https://learn.microsoft.com/pt-br/azure/storage/common/storage-redundancy)

---

## Observações Finais

- Diversas características e recursos de um serviço na nuvem são resumidas nas descrições das plataformas.
- Muitos serviços possuem **links para a documentação oficial**, onde podem ser consultadas informações técnicas e detalhes de implementação.
