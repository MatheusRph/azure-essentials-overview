# Laboratório: Gerenciamento de Custos no Azure pelo Portal

Neste laboratório, vamos explorar as funcionalidades de gerenciamento de custos no Azure, desde a criação de orçamentos até o uso de ferramentas de cálculo e monitoramento. Este guia é prático e envolve várias etapas para configurar limites de gastos, visualizar consumo e gerenciar recursos.

---

## Pré-requisitos
1. Acesso ao [Portal do Azure](https://portal.azure.com).
2. Permissão de Administrador na assinatura Azure ou em uma conta com permissão de "Leitor de Custos".

---

## 1. Criando um Orçamento de Custos

### Passo 1: Acessar o Gerenciamento de Custos
1. No Portal do Azure, acesse **Custo + Gerenciamento**.
2. Clique em **Orçamentos** e selecione **Adicionar Orçamento**.

### Passo 2: Definir o Escopo do Orçamento
1. Escolha a **assinatura** ou **grupo de recursos** para o qual deseja definir um orçamento.
2. Nomeie o orçamento e escolha o período de vigência (mensal, trimestral, etc.).

### Passo 3: Configurar o Limite de Gastos
1. Defina o valor do orçamento de acordo com sua meta de gasto.
2. Configure alertas para receber notificações ao atingir percentuais específicos do limite (50%, 75%, 90%, etc.).
3. Clique em **Criar** para finalizar o orçamento.

---

## 2. Monitorando Consumo e Utilização de Recursos

### Passo 1: Análise de Custos
1. No Portal, vá até **Custo + Gerenciamento** > **Análise de Custos**.
2. Utilize filtros para visualizar os gastos por **recurso**, **grupo de recursos**, ou **serviço**.
3. Ajuste o período de visualização para ver o histórico de consumo mensal, semanal, ou diário.

### Passo 2: Visualização Gráfica e Exportação
1. Analise os gráficos para identificar recursos com altos custos.
2. Exporte os dados em formatos como CSV ou Excel para relatórios externos.

> **Dica:** Use **filtros avançados** para analisar gastos específicos por região ou tipo de serviço.

---

## 3. Usando a Calculadora de Preço e TCO

### Passo 1: Acessar a Calculadora de Preço
1. Acesse a [Calculadora de Preço do Azure](https://azure.microsoft.com/pt-br/pricing/calculator/).
2. Adicione os serviços desejados e ajuste as configurações de uso para ver a previsão de custo.

### Passo 2: Comparar com a Calculadora TCO
1. No [Portal do Azure](https://azure.microsoft.com/pt-br/pricing/tco/calculator/), acesse a Calculadora TCO para comparar os custos do Azure com infraestrutura on-premises.
2. Insira as especificações atuais da infraestrutura para calcular a economia estimada com a migração.

---

## 4. Configurando Tags para Recursos

### Passo 1: Criar e Atribuir Tags
1. No **Portal do Azure**, vá até **Grupos de Recursos** ou **Recursos Individuais**.
2. Selecione **Tags** e insira **Chave** e **Valor** (ex: Chave = "Projeto", Valor = "Marketing").

### Passo 2: Visualizar Custos por Tags
1. Volte para **Análise de Custos** e adicione um filtro de **Tags**.
2. Visualize o custo separado por projetos, departamentos, ou centros de custo conforme as tags configuradas.

---

## 5. Otimizando com Reservas e Monitoramento

### Passo 1: Configurar Instâncias Reservadas
1. Acesse **Custo + Gerenciamento** > **Reservas** no Portal.
2. Selecione um recurso compatível (como VMs ou SQL Database) e configure um plano de reserva para 1 ou 3 anos.
3. Verifique o desconto aplicado automaticamente aos recursos associados.

### Passo 2: Criar Alertas e Notificações
1. Acesse **Monitoramento** > **Alertas** e configure novas regras de alerta para notificar consumo excessivo.
2. Defina condições e ações, como enviar e-mails ou SMS ao ultrapassar o orçamento.

---

Esse laboratório cobre a criação e visualização de custos, o uso de ferramentas de cálculo, o monitoramento de consumo e a configuração de otimização de custos com tags e reservas. Use essas práticas regularmente para manter o controle financeiro e otimizar os investimentos no Azure.
