# processamento_dados_powerBI
Desafio 2 da DIO (módulo 3)- Processamento de Dados Simplificado com Power BI

Descrição do desafio módulo 3 – Processamento de Dados Simplificado com Power BI

1. Criação de uma instância na Azure para MySQL

  -Entrar no site : https://azure.microsoft.com/pt-br/ 
  - Vá até a barra de pesquisa e digite 'MySQL'. Em seguida, clique em 'Servidores de Banco de Dados' onde irá encontrar " Servidores do Banco de Dados do Azure para MySQL";
  - Clicar em criar e assim será exibida a página de Banco de Dados do Azure para MySQL;
  - Escolher o servidor flexivel e clicar em criar;
  - Escolher a assinatura que estou utilizando " Azure subscription 1"
  - O grupo de recursos usado foi o Teste
  - Nome do projeto desafio-projeto2-dio
  - Região East Us
  - Versão My SQL 8
  - tipo de carga de trabalho: Para projetos de desenvolvimento ou hobby
  - Criar o nome de usuário a senha e a confirmação da senha
  - Clicar em avançar : rede >
  - Método de conectividade : Acesso público (endereços IP permitidos) e ponto de extremidade privado
  - Regras de Firewall: Permitir o acesso público de qualquer serviço do Azure de dentro do Azure para esse servidor
  - Clicar em avançar : segurança >
  - Criptografia de dados : Não fazer alterações nesta guia
  - Clicar em avançar : rótulos > Não fazer alterações nesta guia
  - Clicar em avançar : revisar + criar >
  - Clicar em criar
  - Vai começar a ser criada a instância de banco de dados com MySQL





2. Criar o Banco de dados com base disponível no github

   

4. Integração do Power BI com MySQL no Azure

5. Verificar problemas na base a fim de realizar a transformação dos dados

Diretrizes para transformação dos dados

1. Verifique os cabeçalhos e tipos de dados

2. Modifique os valores monetários para o tipo double preciso

3. Verifique a existência dos nulos e analise a remoção

4. Os employees com nulos em Super_ssn podem ser os gerentes. Verifique se há algum colaborador sem gerente

5. Verifique se há algum departamento sem gerente

6. Se houver departamento sem gerente, suponha que você possui os dados e preencha as lacunas

7. Verifique o número de horas dos projetos

8. Separar colunas complexas

9. Mesclar consultas employee e departament para criar uma tabela employee com o nome dos departamentos associados aos colaboradores. A mescla terá como base a tabela employee. Fique atento, essa informação influencia no tipo de junção

10. Neste processo elimine as colunas desnecessárias.

11. Realize a junção dos colaboradores e respectivos nomes dos gerentes . Isso pode ser feito com consulta SQL ou pela mescla de tabelas com Power BI. Caso utilize SQL, especifique no README a query utilizada no processo.

12. Mescle as colunas de Nome e Sobrenome para ter apenas uma coluna definindo os nomes dos colaboradores

13. Mescle os nomes de departamentos e localização. Isso fará que cada combinação departamento-local seja único. Isso irá auxiliar na criação do modelo estrela em um módulo futuro.

14. Explique por que, neste caso supracitado, podemos apenas utilizar o mesclar e não o atribuir.

15. Agrupe os dados a fim de saber quantos colaboradores existem por gerente

16. Elimine as colunas desnecessárias, que não serão usadas no relatório, de cada tabela
