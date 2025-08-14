Análise de gorjetas com python e postgresql

Neste projeto demonstrativo, eu realizo a extração dos dados de um arquivo CSV contendo informações de gorjetas, faço o pré-processamento dos dados e os insiro em uma tabela no postgresql de forma automatizada. 

O projeto mostra, de fato, parte do meu conhecimento. É um projeto que mostra um fluxo de ETL.

O código está em .ipynb para fácil entendimento e testes.


Estrutura do Projeto

    1. Gorjetas/
    ├── gorjetas.ipynb     # arquivo notebook com todo o código
    ├── tips.csv           # base de dados bruta
    ├── .env_sample        # modelo de variáveis de ambiente para você preencher com as suas credenciais 
    └── README.md          # explicação e instruções do projeto 

Configurar variáveis de ambiente
    
    Crie um arquivo .env na pasta 1. Gorjetas baseado no .env_sample:

    DB_NAME=analise_gorjetas
    DB_USER=postgres
    DB_PASSWORD=sua_senha
    DB_HOST=localhost
    DB_PORT=5432

Resultado

    O código trata os dados brutos do CSV, cria a tabela gorjetas no postgresql que zera os dados existentes, e insere os novos dados prontos para consultas SQL ou análises adicionais.