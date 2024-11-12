# Laravel Admin Panel com AdminLTE e JWT Authentication

Este projeto é uma aplicação Laravel com o template AdminLTE 3 integrado e autenticação via JWT. Ele permite que você tenha um painel administrativo com controle de login e rotas de API protegidas por JWT.

## Requisitos

Para rodar este projeto localmente, você precisará de:

- **PHP 8.x ou superior**
- **Composer** - Gerenciador de dependências para PHP
- **Node.js e npm** (para o front-end e dependências do AdminLTE)
- **MySQL** (ou outro banco de dados de sua escolha)
- **Git** (para clonar o repositório)

## Instalação

### Passo 1: Clonar o Repositório

Clone o repositório usando o comando Git:

```bash
git clone https://github.com/MatheuConstantino/laravel-admin-panel.git

### Passo 2: Comandos

Comandos de instalação do projeto

```bash
cd laravel-admin-panel

```bash
composer install

```bash
npm install

### Passo 3: Configuração do banco de dados

Configurando o banco de dados

no arquivo .env
```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=nome_do_banco_de_dados
DB_USERNAME=seu_usuario
DB_PASSWORD=sua_senha

### Passo 3: Gerando a chave da aplicação

```bash
php artisan key:generate

### Passo 4: Executando as migrations

```bash
php artisan migrate

### Passo 4: Chave JWT

Para usar a autenticação via JWT, é necessário configurar a chave secreta do JWT no arquivo .env. Abra o arquivo .env e adicione a seguinte variável (substitua por uma chave segura gerada aleatoriamente):

```bash
JWT_SECRET=SuaChaveSecretaAqui

Você pode gerar a chave por esse comando:
```bash
php artisan jwt:secret

### Passo 5: Executando o frontend

Compile os assets do frontend, com o vite

```bash
npm run dev

### Passo 6: Executando o laravel

```bash
php artisan serve











