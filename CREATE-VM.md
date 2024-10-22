# Criando Máquinas Virtuais no Azure pelo Portal ☁️

Este guia irá te mostrar como criar uma máquina virtual (VM) no Azure usando o portal. Siga os passos abaixo para configurar rapidamente sua nova VM.

## Pré-requisitos ✅

- Uma conta no Microsoft Azure. Se você ainda não tem uma, pode criar uma [aqui](https://azure.microsoft.com/free/).
- Acesso ao [Portal do Azure](https://portal.azure.com).

## Passo a Passo para Criar uma Máquina Virtual 🖥️

### 1. Acesse o Portal do Azure 🌐

- Abra o seu navegador e acesse [portal.azure.com](https://portal.azure.com).
- Faça login com suas credenciais do Azure.

### 2. Criar uma Máquina Virtual ➕

- No painel à esquerda, clique em **"Máquinas Virtuais"**.
- Clique em **"Adicionar"** e, em seguida, em **"Criar uma máquina virtual"**.

### 3. Configure as Configurações Básicas ⚙️

- **Assinatura:** Selecione a assinatura do Azure que deseja usar.
- **Grupo de Recursos:** Crie um novo grupo ou selecione um existente.
- **Nome da VM:** Dê um nome à sua máquina virtual.
- **Região:** Escolha a região onde a VM será criada.
- **Imagem:** Selecione a imagem do sistema operacional que deseja usar (por exemplo, Windows Server ou Ubuntu).
- **Tamanho:** Escolha o tamanho da VM de acordo com suas necessidades. Você pode ver as opções de desempenho e custo.

### 4. Configure as Configurações de Rede 🌐

- **Rede Virtual:** Selecione uma rede virtual existente ou crie uma nova.
- **Sub-rede:** Se necessário, escolha uma sub-rede.
- **IP Público:** Se desejar acesso externo, marque a opção de criar um IP público.

### 5. Configurações de Segurança 🔒

- **Nome de Usuário:** Crie um nome de usuário para acessar a VM.
- **Senha:** Defina uma senha forte. Você também pode optar por autenticação via chave SSH para imagens Linux.
- **Portas de Entrada:** Escolha as portas que deseja abrir (por exemplo, RDP para Windows ou SSH para Linux).

### 6. Revisar + Criar 📄

- Revise todas as configurações que você fez.
- Clique em **"Criar"** para iniciar o provisionamento da sua máquina virtual.

### 7. Acesse sua Máquina Virtual 🔑

- Após a criação, vá para o painel do Azure e selecione **"Máquinas Virtuais"**.
- Clique na sua nova VM.
- Para se conectar, use o cliente RDP (para Windows) ou SSH (para Linux).

## Conclusão 🎉

Parabéns! Você criou sua máquina virtual no Azure. Agora você pode usar essa VM para várias tarefas, como desenvolvimento, teste e hospedagem de aplicativos.

## Recursos Adicionais 📚

- [Documentação Oficial do Azure sobre Máquinas Virtuais](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/quick-create-portal)
- [Tutorial de Conexão Remota](https://learn.microsoft.com/pt-br/azure/virtual-machines/windows/connect-remote-over-rdp)
- [Preços do Azure](https://azure.microsoft.com/pricing/)

---

Se você tiver alguma dúvida ou enfrentar problemas, sinta-se à vontade para consultar a comunidade do Azure ou abrir um chamado de suporte! 🤔💬
