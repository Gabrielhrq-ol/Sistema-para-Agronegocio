# Sistema-de-gerenciamento-Agricula-C-

# 🌾 AgroSistema

Sistema desktop para gerenciamento de operações do agronegócio, desenvolvido em **C# (.NET Framework 4.7.2)** com interface **Windows Forms** e banco de dados **MySQL**.

## Sobre o Projeto

O AgroSistema é uma aplicação de gestão voltada ao agronegócio brasileiro, permitindo o controle centralizado de produtores rurais, fazendas, funcionários, culturas agrícolas e colheitas. O sistema utiliza arquitetura em camadas com separação entre Models, Repositories e Forms.

## Funcionalidades

- **Produtores** — Cadastro e gerenciamento de produtores rurais com validação de CPF
- **Fazendas** — Registro de fazendas com localização (cidade/estado) e área em hectares, vinculadas a um produtor
- **Funcionários** — Controle de funcionários por fazenda, com cargo e salário
- **Culturas** — Cadastro de culturas agrícolas (soja, milho, café, etc.) com tipo e tempo médio de colheita
- **Colheitas** — Registro de plantios e colheitas com data, quantidade em toneladas e observações

## Banco de Dados

MySQL com as seguintes tabelas: `Produtor`, `Fazenda`, `Cultura`, `Funcionario`, `Colheita`.

O script de criação do banco está em `AgroSistema/Database/ScriptParaCriarBanco.sql`.

Já inclui dados iniciais com 5 culturas pré-cadastradas (Soja, Milho, Cana-de-açúcar, Café e Arroz).

## Tecnologias

- C# / .NET Framework 4.7.2
- Windows Forms (WinForms)
- MySQL + MySql.Data (Connector/NET)
- Visual Studio

## Como Executar

1. Clone o repositório
2. Crie o banco de dados executando o script SQL:
