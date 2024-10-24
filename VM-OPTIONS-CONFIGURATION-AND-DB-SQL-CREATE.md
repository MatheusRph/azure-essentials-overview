# Configuração de Instância de Máquina Virtual no Azure

Este guia aborda como configurar uma instância de máquina virtual (VM) no Azure e detalha as principais opções disponíveis durante o processo de criação. As configurações são essenciais para garantir a performance, segurança e gestão correta da sua VM.

## 1. Acessar o Azure Portal
1. Faça login no [Azure Portal](https://portal.azure.com).
2. No painel, clique em **Criar um recurso** e selecione **Máquina Virtual**.

## 2. Configuração Básica da VM

### Informações Básicas
- **Grupo de Recursos**: Escolha um grupo de recursos existente ou crie um novo.
- **Nome da VM**: Escolha um nome significativo para a VM.
- **Região**: Selecione a localização geográfica onde a VM será hospedada. A escolha da região pode afetar a latência e os custos.
- **Disponibilidade**:
  - **Conjunto de Disponibilidade**: Agrupe VMs em domínios de falha e atualização para garantir alta disponibilidade.
  - **Zona de Disponibilidade**: Selecione uma zona específica dentro da região para obter maior tolerância a falhas.

### Opções de Imagem
- **Imagem do Sistema Operacional**: Escolha o sistema operacional que será instalado na VM.
  - Exemplos: **Windows Server 2022**, **Ubuntu 20.04 LTS**, **CentOS**, entre outros.
  - É possível usar **imagens personalizadas** ou **imagens de mercado** disponíveis no Azure Marketplace.

### Tamanho da Máquina Virtual
- Escolha o tamanho da VM com base em suas necessidades de CPU, memória e armazenamento.
  - Exemplos: **B1s** (1 vCPU, 1GB RAM), **D2s_v3** (2 vCPU, 8GB RAM), **E4as_v5** (4 vCPU, 32GB RAM).
  - Use o **Calculador de Preços** do Azure para determinar o custo mensal.

## 3. Configuração de Discos

### Disco do Sistema Operacional
- **Tipo de Disco**:
  - **SSD Premium**: Para cargas de trabalho de alto desempenho.
  - **SSD Padrão**: Para desempenho moderado.
  - **HDD Padrão**: Para workloads leves ou de baixo custo.
  
### Discos de Dados Adicionais
- **Discos Gerenciados**: Crie e anexe discos adicionais para dados, backups ou logs.
- **Desempenho**: Configure o IOPS e o throughput dos discos com base nas necessidades de armazenamento.

## 4. Configuração de Rede

### Rede Virtual (VNet)
- **Rede Virtual**: Selecione uma rede virtual existente ou crie uma nova.
- **Sub-rede**: Escolha ou crie uma sub-rede onde a VM será implantada.

### Endereço IP Público
- **Alocar IP Público**: Se necessário, escolha um **IP estático** ou **dinâmico** para a VM.
  - **Estático**: O endereço IP permanece fixo.
  - **Dinâmico**: O endereço IP pode mudar entre reinicializações.

### Grupo de Segurança de Rede (NSG)
- **NSG**: Configura regras de firewall para controle de tráfego.
  - **Portas de Entrada**: Configure as portas que serão abertas (ex.: 80/443 para HTTP/HTTPS, 22 para SSH, 3389 para RDP).
  - **Portas de Saída**: Defina regras de saída para restringir ou permitir o tráfego da VM para a internet.

### Balanceamento de Carga (Opcional)
- **Balanceador de Carga**: Adicione a VM a um balanceador de carga para distribuir o tráfego de rede em várias instâncias de VM.
  - Escolha entre **Balanceador de Carga Interno** (para redes internas) ou **Balanceador de Carga Público** (para tráfego da internet).

## 5. Gerenciamento

### Diagnósticos de Boot
- **Habilitar Diagnóstico de Boot**: Registra informações sobre o processo de inicialização da VM, útil para identificar problemas de inicialização.

### Agentes de Extensão
- **Instalar Extensões**: Utilize extensões para automatizar tarefas como backup, monitoramento e gerenciamento de antivírus.
  - Exemplos: **Azure Backup**, **Log Analytics**, **Custom Script Extension**.

### Tags
- **Tags**: Adicione tags para categorizar e identificar recursos com chave/valor (ex: `Projeto:Financeiro`, `Ambiente:Produção`).

## 6. Configurações Avançadas

### Disponibilidade e Redundância
- **Conjunto de Dimensionamento**: Crie várias instâncias de VM para escalabilidade automática.
- **Snapshot de VM**: Habilite snapshots para criar backups da VM para recuperação rápida em caso de falha.

### Autenticação e Segurança
- **Autenticação SSH ou RDP**:
  - **SSH (para Linux)**: Adicione sua chave pública SSH para acessar a VM de forma segura.
  - **RDP (para Windows)**: Defina um nome de usuário e senha para login remoto via Remote Desktop Protocol.
  
### Identity Management
- **Managed Identity**: Permite que a VM interaja com outros serviços do Azure sem necessidade de credenciais explícitas.
  - **User-Assigned Managed Identity**: Associado a várias VMs.
  - **System-Assigned Managed Identity**: Gerado automaticamente pela VM.

## 7. Revisar e Criar

Após definir todas as configurações, clique em **Revisar e Criar** para revisar as opções escolhidas. Verifique os custos estimados e clique em **Criar** para implantar a VM.

---

## Criação de Instância de Banco de Dados no Azure SQL

Para criar uma instância de banco de dados, siga o guia completo no [Azure SQL Quickstart](https://learn.microsoft.com/pt-br/azure/azure-sql/database/single-database-create-quickstart?view=azuresql&tabs=azure-portal).

1. No **Azure Portal**, clique em **Criar um recurso** > **Banco de Dados** > **SQL Database**.
2. Configure as opções, como nome do banco de dados, servidor, grupo de recursos e redundância de backup.
3. Após a criação, use ferramentas como **Azure Data Studio** ou **SQL Server Management Studio (SSMS)** para gerenciar o banco.

---

### Referências
- [Responsabilidades Compartilhadas no Azure](https://learn.microsoft.com/pt-br/azure/security/fundamentals/shared-responsibility)
- [Criação de Banco de Dados Azure SQL](https://learn.microsoft.com/pt-br/azure/azure-sql/database/single-database-create-quickstart?view=azuresql&tabs=azure-portal)
