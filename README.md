# 🚗 Projeto de Gerenciamento de Veículos
Este projeto é uma aplicação web para gerenciamento de veículos, utilizando um backend em Node.js com Express, um banco de dados MySQL, e integração com WordPress. A aplicação permite realizar operações CRUD (Create, Read, Update, Delete) nos veículos registrados.

## 📑 Índice
1. [Funcionalidades](#%EF%B8%8F-funcionalidades)
2. [Tecnologias Utilizadas](#-tecnologias-utilizadas)
3. [Pré-requisitos](#-pré-requisitos)
4. [Instalação](#-instalação)
5. [Autor](#-autor)

## ⚙️ Funcionalidades

- [X] Listar Veículos: Obter todos os veículos cadastrados.
- [X] Buscar Veículo por ID: Recuperar informações de um veículo específico.
- [X] Adicionar/Editar Veículo: Inserir um novo veículo ou atualizar informações de um veículo existente.
- [X] Excluir Veículo: Remover um veículo do banco de dados.
      
## 🛠 Tecnologias Utilizadas

- Node.js: Ambiente de execução JavaScript do lado do servidor.
- Express: Framework web para Node.js que facilita a criação de APIs.
- MySQL: Sistema de gerenciamento de banco de dados utilizado para armazenar os dados dos veículos.
- WordPress: Sistema de gerenciamento de conteúdo que pode ser integrado ao projeto, permitindo a gestão de conteúdo relacionado.

## 📝 Pré-requisitos

Para executar este projeto, você precisará de:

* Node.js instalado.
* MySQL instalado e em funcionamento.
* Uma instalação do WordPress, se desejar integrar.
* IDE de sua escolha (Visual Studio Code, etc.).

## 🚀 Instalação

#### 1. Clone o repositório:

```bash
git clone https://github.com/iSamuel22/gerenciamento-veiculos.git
```

#### 2. Navegue até o diretório do projeto:

```bash
cd gerenciamento-veiculos
```

#### 3. Instale as dependências:

```bash
npm install
```

#### 4. Configure o Banco de Dados:

Crie um banco de dados no MySQL chamado agenda e execute o seguinte comando para criar a tabela de veículos:

```sql
CREATE TABLE VEICULOS (
    ID INT AUTO_INCREMENT PRIMARY KEY,
    DESCRICAO VARCHAR(255) NOT NULL,
    PORTAS INT,
    COR VARCHAR(50)
);
```

#### 5. Configure as Variáveis de Ambiente:

Crie um arquivo `.env` na raiz do projeto e defina as variáveis de configuração do banco de dados:

```plaintext
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=mysql
DB_NAME=agenda
```

#### 6. Execute o Servidor:

```bash
npm start ou npm run dev
```

## 👤 Autor
Desenvolvido por _Samuel Ildebrando Pena._
