# 🏁 API de Fórmula 1 🏁

Este projeto é uma API simples construída com [Fastify](https://fastify.dev/) e [@fastify/cors](https://github.com/fastify/fastify-cors) que fornece informações sobre equipes e pilotos de Fórmula 1.  
Ideal para estudos de APIs REST com Node.js.

---

## 📌 Tecnologias Utilizadas

- **[Node.js](https://nodejs.org/)** — Ambiente de execução JavaScript no lado do servidor  
- **[TypeScript](https://www.typescriptlang.org/)** — Superset do JavaScript com tipagem estática  
- **[Fastify](https://fastify.dev/)** — Framework web rápido e leve para Node.js  
- **[@fastify/cors](https://github.com/fastify/fastify-cors)** — Plugin para habilitar CORS no Fastify  
- **[tsx](https://github.com/esbuild-kit/tsx)** — Executa arquivos TypeScript/ESM sem compilação prévia  
- **[tsup](https://tsup.egoist.dev/)** — Empacotador rápido para TypeScript/JavaScript  
- **[@types/node](https://www.npmjs.com/package/@types/node)** — Tipos TypeScript para APIs do Node.js  

---

## 🚀 Como Executar o Projeto

### 1️⃣ Clonar o repositório
```bash
git clone https://github.com/Jezebel1990/node-f1.git

```

## 2️⃣ Instalar as dependências
```bash
npm install
```

### 3️⃣ Iniciar o servidor
```bash
npm run start:dev
```

O servidor iniciará em:
`http://localhost:3333`

---
## 📡 Endpoints Disponíveis
🔹 Listar todas as equipes
`GET /teams`

**Exemplo de resposta:**
```json
{
  "teams": [
    { "id": 1, "name": "McLaren", "base": "Woking, United Kingdom" },
    { "id": 2, "name": "Mercedes", "base": "Brackley, United Kingdom" }
  ]
}
```

🔹 Listar todos os pilotos
`GET /drivers`

**Exemplo de resposta:**
```json

{
  "drivers": [
    { "id": 1, "name": "Max Verstappen", "team": "Red Bull Racing" },
    { "id": 2, "name": "Lewis Hamilton", "team": "Ferrari" }
  ]
}
```

🔹 Buscar piloto por ID
`GET /drivers/:id`


**Exemplo:**

`GET /drivers/1`


**Exemplo de resposta:**
```json

{
  "driver": { "id": 1, "name": "Max Verstappen", "team": "Red Bull Racing" }
}
```

---
Feito com ♥ por [Jezebel Guedes](https://www.linkedin.com/in/jezebel-guedes/) 👋 Entre em contato!