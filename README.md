# 🎧 Gerenciador de Podcasts

API REST para gerenciamento de podcasts desenvolvida em Node.js com TypeScript, construída do zero sem frameworks para demonstrar o funcionamento interno de uma aplicação web.

## 📋 Funcionalidades

- Listar todos os episódios de podcasts
- Filtrar episódios por parâmetros específicos
- Estrutura modular com controllers, services e repositories

## 🚀 Tecnologias

- **Node.js** - Runtime JavaScript
- **TypeScript** - Superset tipado do JavaScript
- **TSX** - Executor TypeScript para desenvolvimento
- **TSUP** - Bundler TypeScript

## 📁 Estrutura do Projeto

```
src/
├── controllers/     # Controladores da aplicação
├── models/         # Modelos de dados
├── repositories/   # Camada de dados
├── routes/         # Definição de rotas
├── services/       # Lógica de negócio
├── utils/          # Utilitários
├── app.ts          # Configuração da aplicação
└── server.ts       # Servidor HTTP
```

## 🔧 Instalação

1. Clone o repositório:
```bash
git clone <url-do-repositorio>
cd dp-gerenciador-podcasts
```

2. Instale as dependências:
```bash
npm install
```

3. Configure as variáveis de ambiente:
```bash
# O arquivo .env já está configurado com:
PORT=3333
```

## ▶️ Como Executar

### Desenvolvimento
```bash
# Modo desenvolvimento
npm run start:dev

# Modo watch (reinicia automaticamente)
npm run start:watch
```

### Produção
```bash
# Gerar build
npm run dist

# Executar build
npm run start:dist
```

## 📡 Endpoints da API

### Listar Episódios
```http
GET /api/list
```
Retorna todos os episódios de podcasts disponíveis.

### Filtrar Episódios
```http
GET /api/episode?[parametros]
```
Retorna episódios filtrados por parâmetros específicos.

## 📝 Exemplo de Resposta

```json
[
  {
    "podcastName": "Nome do Podcast",
    "episode": "Título do Episódio",
    "videoId": "ID_do_Video",
    "categories": ["categoria1", "categoria2"]
  }
]
```

## 🛠️ Scripts Disponíveis

- `npm run start:dev` - Inicia o servidor em modo desenvolvimento
- `npm run start:watch` - Inicia com watch mode
- `npm run dist` - Gera build de produção
- `npm run start:dist` - Executa o build de produção

## 📄 Licença

Este projeto está sob a licença ISC.