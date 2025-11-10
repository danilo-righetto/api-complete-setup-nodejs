# 🚀 Setup completo: Back-end Node.js com TypeScript, Fastify e Biome do zero

Este projeto apresenta uma configuração **completa e moderna** para iniciar rapidamente o desenvolvimento de back-ends com **Node.js**, **TypeScript**, **Fastify** e **Biome**.  
A base foi construída para garantir **performance, escalabilidade, qualidade de código e produtividade** desde o primeiro commit.

---

## 🧩 Tecnologias e Ferramentas Principais

- **[Node.js](https://nodejs.org/)** — Ambiente de execução JavaScript.
- **[TypeScript](https://www.typescriptlang.org/)** — Tipagem estática e melhor experiência de desenvolvimento.
- **[Fastify](https://fastify.dev/)** — Framework web rápido e altamente extensível.
- **[pnpm](https://pnpm.io/)** — Gerenciador de pacotes rápido e eficiente.
- **[Biome](https://biomejs.dev/)** — Linter, formatter e ferramenta de análise tudo-em-um.
- **ESM (ECMAScript Modules)** — Suporte nativo a módulos modernos do Node.js.

---

## ⚙️ Estrutura do Projeto

📦 setup-backend-node-fastify

```sh
├── src/
│ ├── server.ts # Ponto de entrada da aplicação
│ ├── app.ts # Instância e configuração do Fastify
│ ├── routes/
│ │ └── example.route.ts
│ ├── controllers/
│ │ └── example.controller.ts
│ ├── plugins/
│ │ └── cors.ts # Exemplo de plugin global
│ └── utils/
│ └── logger.ts # Configuração de logs
│
├── .biome.json # Configuração do Biome (lint + format)
├── tsconfig.json # Configuração do TypeScript
├── package.json
├── pnpm-lock.yaml
└── README.md
```

---

## 🧱 Pré-requisitos

Antes de começar, verifique se possui instalado:

- [Node.js >= 20](https://nodejs.org/en/)
- [pnpm >= 10.20.0](https://pnpm.io/installation)
- [biome >= 2.3.4](https://biomejs.dev/pt-br/)
- [zod >= 4.1.12](https://zod.dev/)

### Biome

Instalando o [biome](https://biomejs.dev/pt-br/) no projeto:

```sh
pnpm add -D -E @biomejs/biome
```

Configurando o [biome](https://biomejs.dev/pt-br/) no projeto:

```sh
pnpm exec biome init
```

Usando o [biome](https://biomejs.dev/pt-br/) no projeto:

```sh
# Formatar todos os arquivos
pnpm exec biome format --write

# Formatar arquivos específicos
pnpm exec biome format --write <files>

# Fazer lint e aplicar correções seguras a todos os arquivos
pnpm exec biome lint --write

# Fazer lint nos arquivos e aplicar correções seguras a arquivos específicos
pnpm exec biome lint --write <files>

# Formatar, fazer lint e organizar importações de todos os arquivos
pnpm exec biome check --write

# Formatar, fazer lint e organizar importações de arquivos específicos
pnpm exec biome check --write <files>
```

---

## 🚀 Instalação e Execução

Clone o repositório e instale as dependências:

```sh
git clone https://github.com/danilo-righetto/api-complete-setup-nodejs.git
cd api-complete-setup-nodejs
pnpm install
```

## 🧰 Scripts Disponíveis

Comando	/ Descrição
- `pnpm dev`	Executa o servidor em modo desenvolvimento com hot reload
- `pnpm build`	Compila o código TypeScript para JavaScript (dist/)
- `pnpm start`	Inicia o servidor a partir dos arquivos compilados
- `pnpm lint`	Executa o linting de código com Biome
- `pnpm format`	Formata o código automaticamente com Biome
- `pnpm check`	Verifica erros de estilo e tipagem

## 🧠 Conceito e Filosofia

Este setup foi criado para ser a base de projetos Node.js modernos, com foco em:

🚀 Performance — Fastify é um dos frameworks HTTP mais rápidos do ecossistema Node.

💪 Escalabilidade — Estrutura modular e de fácil manutenção.

🧼 Qualidade — Biome garante consistência de código e boas práticas.

⚡ Produtividade — Configuração pronta para uso imediato com scripts automatizados.

🧩 Extensibilidade — Facilmente adaptável a bancos de dados, autenticação e testes.

## 🧪 Extensões Recomendadas (VS Code)

Para uma melhor experiência de desenvolvimento, instale as seguintes extensões:

Biome — Linter e formatter integrados (biomejs.biome).

TypeScript ESLint Support — Autocompletar e detecção de tipos.

REST Client ou Thunder Client — Testes rápidos de rotas HTTP.

Error Lens — Exibição imediata de erros e avisos no editor.

## 🧩 Boas Práticas

Utilize import/export ES Modules nativos.

Mantenha cada rota isolada em seu próprio arquivo dentro de /routes.

Centralize dependências de terceiros em /plugins.

Evite lógica de negócio dentro das rotas — use controllers e services.

Valide entradas com o schema validator nativo do Fastify.

## 🧱 Compilação e Deploy

Gere o build de produção com:

```sh
pnpm build
```

Isso criará a pasta /dist, que contém os arquivos prontos para execução:

```sh
pnpm start
```

## API Docs - Screenshots

![Scalar API Documentation](./img/scalar-api-doc.png)

## ⚙️ Fonte

- [Rocketseat - Setup completo: Back-end Node.js com TypeScript, Fastify e Biome do zero](https://www.youtube.com/watch?v=usN5-uDCc9Q)

## 🧾 Licença

Este projeto é distribuído sob a licença **GNU AFFERO**.
Sinta-se à vontade para usar, modificar e compartilhar conforme suas necessidades.

## ✨ Autor

Desenvolvido com 💻 por [Danilo Righetto](https://github.com/danilorighetto)

Tech Lead na [Code Cuber](https://www.instagram.com/codecuber)