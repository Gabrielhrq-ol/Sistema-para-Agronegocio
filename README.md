<div align="center">

# 🌾 AgroSistema

Sistema desktop para gerenciamento de operações do agronegócio brasileiro

![C#](https://img.shields.io/badge/C%23-.NET%204.7.2-purple?style=flat-square&logo=csharp)
![WinForms](https://img.shields.io/badge/Interface-WinForms-blue?style=flat-square)
![MySQL](https://img.shields.io/badge/Banco-MySQL-orange?style=flat-square&logo=mysql)
![Status](https://img.shields.io/badge/Status-Concluído-green?style=flat-square)

</div>

---

## 📋 Sobre o Projeto

O **AgroSistema** é uma aplicação desktop de gestão voltada ao agronegócio brasileiro, que permite o controle centralizado de produtores rurais, fazendas, funcionários, culturas agrícolas e colheitas.

Desenvolvido como **projeto acadêmico** em grupo de 5 integrantes no curso de Sistemas de Informação da **UNIARA**, com divisão de responsabilidades por módulos e arquitetura em camadas (Models, Repositories e Forms).

---

## ⚙️ Funcionalidades

| Módulo | Descrição |
|---|---|
| 👨‍🌾 **Produtores** | Cadastro e gerenciamento de produtores rurais com validação de CPF |
| 🏡 **Fazendas** | Registro com localização (cidade/estado) e área em hectares, vinculadas a um produtor |
| 👷 **Funcionários** | Controle por fazenda, com cargo e salário |
| 🌱 **Culturas** | Cadastro de culturas agrícolas (soja, milho, café, etc.) com tipo e tempo médio de colheita |
| 🌾 **Colheitas** | Registro de plantios e colheitas com data, quantidade em toneladas e observações |

---

## 👨‍💻 Minha Contribuição

Fui responsável pelo desenvolvimento completo do **módulo de Produtores**, que inclui:

- ✅ CRUD completo (cadastro, edição, exclusão e listagem)
- ✅ Validação de CPF com algoritmo dos dois dígitos verificadores
- ✅ Validação de e-mail
- ✅ Proteção de integridade referencial (impede exclusão de produtor com fazendas vinculadas)
- ✅ Integração com banco de dados via padrão Repository usando Dapper

---

## 🛠️ Tecnologias

| Tecnologia | Uso |
|---|---|
| C# / .NET Framework 4.7.2 | Linguagem e plataforma principal |
| Windows Forms (WinForms) | Interface gráfica |
| MySQL + MySql.Data | Banco de dados e conector |
| Dapper | Micro-ORM para acesso ao banco |
| Visual Studio | IDE de desenvolvimento |

---

## 📁 Estrutura do Projeto

``````
AgroSistema/
├── Forms/           # Telas da aplicação (WinForms)
├── Models/          # Entidades do sistema
├── Repositories/    # Acesso ao banco de dados
├── Database/        # Script SQL de criação do banco
└── Program.cs       # Ponto de entrada da aplicação
``````

---

## 🚀 Como Executar

**Pré-requisitos:** Visual Studio, MySQL instalado e rodando.

``````bash
# 1. Clone o repositório
git clone https://github.com/Gabrielhrq-ol/Sistema-para-Agronegocio.git
``````

**2.** Execute o script SQL para criar o banco de dados no MySQL:
``````
AgroSistema/Database/ScriptParaCriarBanco.sql
``````
> O script já inclui 5 culturas pré-cadastradas: Soja, Milho, Cana-de-açúcar, Café e Arroz.

**3.** Configure a string de conexão em `AgroSistema/Repositories/Conexao.cs` com seu host, usuário e senha do MySQL.

**4.** Abra o projeto no Visual Studio pelo arquivo `AgroSistema.slnx` e execute com **F5**.

---

## 👥 Equipe

Projeto desenvolvido em grupo de 5 integrantes como atividade acadêmica do curso de **Sistemas de Informação — UNIARA**.