🌾 AgroSistema
Sistema desktop para gerenciamento de operações do agronegócio, desenvolvido em C# (.NET Framework 4.7.2) com interface Windows Forms e banco de dados MySQL.

Sobre o Projeto
O AgroSistema é uma aplicação de gestão voltada ao agronegócio brasileiro, permitindo o controle centralizado de produtores rurais, fazendas, funcionários, culturas agrícolas e colheitas.
O sistema foi desenvolvido como projeto acadêmico em grupo de 5 integrantes, com divisão de responsabilidades por módulos. A arquitetura adota separação em camadas: Models, Repositories e Forms.

Minha Contribuição
Fui responsável pelo desenvolvimento completo do módulo de Produtores, que inclui:

CRUD completo (cadastro, edição, exclusão e listagem)
Validação de CPF com implementação do algoritmo dos dois dígitos verificadores
Validação de e-mail
Proteção de integridade referencial (impede exclusão de produtor com fazendas vinculadas)
Integração com o banco de dados via padrão Repository usando Dapper


Funcionalidades do Sistema

Produtores — Cadastro e gerenciamento de produtores rurais com validação de CPF
Fazendas — Registro de fazendas com localização (cidade/estado) e área em hectares, vinculadas a um produtor
Funcionários — Controle de funcionários por fazenda, com cargo e salário
Culturas — Cadastro de culturas agrícolas (soja, milho, café, etc.) com tipo e tempo médio de colheita
Colheitas — Registro de plantios e colheitas com data, quantidade em toneladas e observações


Banco de Dados
MySQL com as seguintes tabelas: Produtor, Fazenda, Cultura, Funcionario, Colheita.
O script de criação está em AgroSistema/Database/ScriptParaCriarBanco.sql e já inclui 5 culturas pré-cadastradas (Soja, Milho, Cana-de-açúcar, Café e Arroz).

Tecnologias

C# / .NET Framework 4.7.2
Windows Forms (WinForms)
MySQL + MySql.Data (Connector/NET)

Como Executar

Clone o repositório
Crie o banco de dados executando o script SQL no MySQL:

AgroSistema/Database/ScriptParaCriarBanco.sql

Configure a string de conexão em AgroSistema/Repositories/Conexao.cs com seu host, usuário e senha do MySQL
Abra o projeto no Visual Studio pelo arquivo AgroSistema.slnx
Execute pressionando F5 ou clicando em Iniciar


Estrutura do Projeto
AgroSistema/
├── Forms/          # Telas da aplicação (WinForms)
├── Models/         # Entidades do sistema
├── Repositories/   # Acesso ao banco de dados
├── Database/       # Script SQL de criação do banco
└── Program.cs      # Ponto de entrada da aplicação

Equipe
Projeto desenvolvido em grupo de 5 integrantes como atividade acadêmica do curso de Sistemas de Informação — UNIARA
