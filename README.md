# SDW2023_ETLproject

**Contexto:** Este projeto visa desenvolver um processo de ETL (Extract, Transform, Load).

Para evitar a necessidade de usar uma API, criaremos uma coleção de dados falsos contendo informações pessoais de clientes de um banco e um histórico de transações de 30 dias para cada cliente, incluindo detalhes sobre onde e quanto gastaram.

Nosso objetivo é classificar os locais onde as transações ocorreram usando machine learning (ML) e, em seguida, adicionar essa categoria às transações.

Além disso, usaremos os dados atualizados das transações de cada cliente para gerar um gráfico de porcentagem de gastos por categoria, revelando o padrão de gastos de cada um.

**Condições do Problema:**

1- Simularemos uma coleção de dados com informações pessoais dos clientes, incluindo: `[ClienteID, Nome, Sobrenome, Idade, CPF, Gênero, Telefone, Email, CEP, Estado, Cidade, Endereço, Limite de Crédito, Saldo]`.

2- Simularemos um histórico de transações bancárias para cada cliente contendo: `[TransacaoID, ClienteID, Saldo Inicial, Limite de Crédito Inicial, Tipo de Transação, Data da Transação, Estabelecimento, Valor, Saldo Atualizado, Limite de Crédito Atualizado]`. Utilizaremos o chatGPT para gerar nomes fictícios de empresas onde as transações ocorreram. Após as transações, atualizaremos os novos saldos e limites de crédito no arquivo de dados pessoais.

3- Usaremos ML para classificar os estabelecimentos em categorias: [Lazer, Alimentação, Casa, Saúde, Serviços de Streaming, Vestuário, Outros] com base no arquivo de transações de cada cliente e adicionaremos essa informação às transações.

4- Geraremos um histograma individual para cada cliente, classificando seus gastos.
