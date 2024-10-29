# Resumo de Laboratório - Utilizando Serviços de Armazenamento no Azure

## 1. Acessando o Portal do Azure

- **Criar uma Conta**: 
  - Acesse o [Portal do Azure](https://azure.microsoft.com/).
  - Crie uma conta gratuita.

- **Login**: 
  - Após criar sua conta, faça login usando suas credenciais.

## 2. Criando uma Conta de Armazenamento

1. No painel do Azure, clique em **Criar um recurso**.
2. Selecione **Armazenamento** > **Conta de Armazenamento**.
3. Preencha os campos necessários:
   - **Nome da Conta**: Deve ser único em todo o Azure.
   - **Tipo de Conta**: Selecione "General Purpose v2" para acesso a todos os serviços de armazenamento.
   - **Região**: Escolha a região mais próxima para minimizar latência.
   - **Desempenho**: Selecione entre Standard ou Premium, dependendo das necessidades da sua aplicação.
   - **Redundância**: Escolha o tipo de redundância (LRS, GRS, etc.).
4. Clique em **Revisar + criar** e depois em **Criar**.

## 3. Criando Recursos de Armazenamento

### Azure Blob Storage
1. No painel do Azure, clique em **Criar um recurso** > **Armazenamento** > **Blob Storage**.
2. Escolha a conta de armazenamento que você criou anteriormente.
3. Defina as configurações:
   - Tipo de desempenho
   - Camada de acesso (Frequent, Cool, Archive)
4. Após a criação, faça upload de blobs usando a interface do portal ou ferramentas como **AzCopy**.

### Azure Disk Storage
1. Clique em **Criar um recurso** > **Armazenamento** > **Disco**.
2. Selecione a conta de armazenamento desejada.
3. Escolha o tipo de disco (HDD, SSD, etc.) e configure opções de tamanho.
4. Após criar o disco, você pode anexá-lo a uma VM.

### Azure File Storage
1. Acesse **Criar um recurso** > **Armazenamento** > **File Share**.
2. Selecione a conta de armazenamento que você criou.
3. Configure o nome e as quotas de armazenamento.
4. Use o SMB para mapear o compartilhamento em máquinas virtuais.

## 4. Consultando e Gerenciando Armazenamento

- **Navegação**: 
  - Vá até **Todos os recursos** para visualizar seus serviços de armazenamento.
  
- **Configurações**: 
  - Clique no recurso específico para acessar opções como **Configurações**, **Cópias de segurança** e **Monitoramento**.

- **Consultas**: 
  - Para Azure Table Storage, use o **Azure Storage Explorer** ou o portal para executar consultas.

## 5. Utilizando o Azure Data Box

1. **Solicitar um Data Box**: 
   - No portal, navegue até **Criar um recurso** > **Armazenamento** > **Data Box**.
   - Siga as instruções para solicitar o dispositivo.

2. **Transferir Dados**: 
   - Após receber o Data Box, transfira os dados conforme as instruções enviadas.

3. **Devolução**: 
   - Devolva o Data Box conforme as orientações.

## 6. Migração de Dados

### Azure Migrate
1. No portal, acesse **Criar um recurso** > **Migração** > **Azure Migrate**.
   - Inicie o processo de migração e receba recomendações.

### Azure Database Migration Service
1. Navegue até **Criar um recurso** > **Banco de Dados** > **Serviço de Migração de Banco de Dados**.
   - Comece a migração de bancos de dados.

## 7. Consultando a Documentação da Microsoft

- Acesse a [Documentação do Azure](https://learn.microsoft.com/pt-br/azure/) para mais detalhes e guias.
- Consulte páginas específicas:
  - [Azure Blob Storage](https://learn.microsoft.com/pt-br/azure/storage/blobs/)
  - [Azure Disk Storage](https://learn.microsoft.com/pt-br/azure/storage/disks/)
  - [Azure Data Box](https://learn.microsoft.com/pt-br/azure/databox/)

## Dicas Adicionais
- Utilize a **Busca** no portal do Azure para encontrar serviços e documentação específica.
- Verifique a seção **Aprendizado** no portal para cursos e tutoriais sobre os serviços do Azure.
