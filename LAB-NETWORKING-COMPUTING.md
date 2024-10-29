# README - Criando Serviços de Computação e Rede no Azure

Este documento oferece um guia detalhado para criar e gerenciar serviços de computação e rede no Microsoft Azure através do Portal Azure. Este guia cobre desde máquinas virtuais até serviços de rede, incluindo VPNs, balanceamento de carga e Kubernetes. Vamos explorar cada serviço e suas opções no portal.

---

## Criando Máquinas Virtuais (VMs) no Portal Azure

### Passo 1: Acessar o Portal Azure
1. Abra seu navegador e acesse [portal.azure.com](https://portal.azure.com).
2. Faça login com suas credenciais do Azure.

### Passo 2: Criar uma Máquina Virtual
1. No painel à esquerda, clique em **"Máquinas Virtuais"**.
2. Clique em **"Adicionar"** e, em seguida, em **"Criar uma máquina virtual"**.

### Passo 3: Configurar as Configurações Básicas
- **Assinatura**: Selecione a assinatura desejada.
- **Grupo de Recursos**: Crie um novo ou selecione um existente.
- **Nome da VM**: Dê um nome à sua máquina virtual.
- **Região**: Escolha a região onde a VM será criada.
- **Imagem**: Selecione o sistema operacional (ex: Windows Server, Ubuntu, etc.).
- **Tamanho**: Selecione o tamanho da VM. Você pode escolher entre diferentes tipos de máquinas (Standard, B-series, etc.) dependendo da carga de trabalho.

### Passo 4: Configurações de Rede
1. **Rede Virtual**: Selecione uma rede virtual existente ou crie uma nova.
2. **Sub-rede**: Escolha uma sub-rede para a VM.
3. **IP Público**: Crie um IP público se precisar de acesso externo.
4. **Grupos de Segurança de Rede**: Configure as regras de firewall para controlar o tráfego de entrada e saída.

### Passo 5: Configurações de Segurança
- **Nome de Usuário**: Crie um nome de usuário para acesso à VM.
- **Senha**: Defina uma senha forte.
- **Portas de Entrada**: Escolha as portas que deseja abrir (ex: RDP para Windows ou SSH para Linux).

### Passo 6: Revisar e Criar
1. Revise suas configurações.
2. Clique em **"Criar"** para provisionar a VM.

### Recursos Adicionais:
- [Documentação sobre Máquinas Virtuais](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)

---

## Configurando Serviços de Rede

### Balanceamento de Carga (Load Balancing)
1. No portal, vá para **"Todos os serviços"** e busque por **"Balanceadores de Carga"**.
2. Clique em **"Adicionar"** para criar um novo balanceador.
3. Selecione o tipo de balanceador:
   - **Load Balancer**: Distribui o tráfego entre VMs em uma única região.
   - **Traffic Manager**: Balanceador baseado em DNS para gerenciar o tráfego global.

#### Configurações do Balanceador de Carga
- **Nome**: Dê um nome ao balanceador.
- **Região**: Selecione a região.
- **SKU**: Escolha entre Standard ou Basic.
- **Regras de Balanceamento**: Defina regras de balanceamento para direcionar o tráfego.

### Gateway VPN e ExpressRoute
1. Busque por **"Gateways de VPN"** no portal.
2. Clique em **"Adicionar"** para criar um novo gateway.
3. Configure as seguintes opções:
   - **Nome**: Dê um nome ao gateway.
   - **Tipo de VPN**: Escolha entre VPN baseada em rota ou política.
   - **SKU**: Selecione o SKU apropriado (ex: Basic, VpnGw1, etc.).
   - **Rede Virtual**: Selecione ou crie uma nova rede virtual.

#### ExpressRoute
- Para uma conexão dedicada ao Azure, procure por **"ExpressRoute"** e siga o processo de configuração que inclui a escolha do circuito e as configurações de peering.

### Serviço DNS do Azure
1. No portal, busque por **"DNS Zones"**.
2. Clique em **"Adicionar"** para criar uma nova zona DNS.
3. Preencha as informações:
   - **Nome da Zona**: Defina o nome do domínio.
   - **Grupo de Recursos**: Escolha um existente ou crie um novo.

### Configuração de DNS
- Crie registros DNS (A, CNAME, MX) conforme necessário para mapear seu domínio aos recursos do Azure.

### Comparação entre VMs, Contêineres e Azure Virtual Desktop
- **Máquinas Virtuais**: Para cargas de trabalho tradicionais, como aplicativos legados.
- **Contêineres**: Para aplicativos modernos que requerem escalabilidade rápida e isolamento, como Docker.
- **Azure Virtual Desktop**: Ideal para ambientes de trabalho virtualizados e acessos remotos.

### Criando um Cluster AKS (Azure Kubernetes Service)
1. Busque por **"Kubernetes Services"** no portal.
2. Clique em **"Adicionar"** para criar um novo cluster.
3. Configure as opções:
   - **Nome do Cluster**: Dê um nome ao cluster.
   - **Região**: Escolha a região desejada.
   - **Tamanho do Nó**: Selecione o número de nós e o tamanho.
   - **Configurações de Rede**: Escolha uma rede virtual existente ou crie uma nova.

### Criando e Gerenciando Contêineres
1. Busque por **"Container Instances"**.
2. Clique em **"Adicionar"** para criar uma nova instância de contêiner.
3. Preencha as informações:
   - **Nome**: Defina um nome para o contêiner.
   - **Imagem do Contêiner**: Especifique a imagem a ser utilizada.
   - **Recursos**: Selecione o tamanho da instância e as configurações de rede.

### Azure Functions
1. Acesse **"Funções do Azure"** no portal.
2. Clique em **"Adicionar"** para criar uma nova função.
3. Configure:
   - **Nome da Função**: Defina um nome.
   - **Assinatura**: Escolha a assinatura do Azure.
   - **Grupo de Recursos**: Selecione ou crie um novo grupo.
   - **Tipo de Ambiente de Execução**: Escolha entre .NET, Node.js, Python, etc.

---

## Referências e Recursos Adicionais
- [Documentação Completa do Azure](https://learn.microsoft.com/pt-br/azure/)
- [Guia de Balanceamento de Carga no Azure](https://learn.microsoft.com/pt-br/azure/load-balancer/)
- [Guia de Configuração do Gateway VPN](https://learn.microsoft.com/pt-br/azure/vpn-gateway/vpn-gateway-howto-vnet-vpn)
- [Documentação sobre Azure Kubernetes Service](https://learn.microsoft.com/pt-br/azure/aks/)
- [Documentação do Azure Functions](https://learn.microsoft.com/pt-br/azure/azure-functions/)

---

Este guia fornece uma visão completa sobre como criar e configurar serviços de computação e rede no Azure, permitindo que você implemente uma arquitetura robusta e escalável na nuvem.
