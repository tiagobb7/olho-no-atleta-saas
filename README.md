# Olho no Atleta SaaS

Este repositório contém o boilerplate inicial do SaaS “Casa Olho no Atleta”.

## Estrutura

- **src/**: código-fonte principal  
- **docker-compose.yml**: orquestra serviços de dev e banco  
- **.github/workflows/ci.yml**: pipeline de CI via GitHub Actions  
- **package.json**: dependências e scripts npm

## Como rodar localmente

1. Clone o repositório localmente.
2. Instale dependências:
   ```bash
   npm install
   ```
3. Inicie serviços:
   ```bash
   docker-compose up --build
   ```
4. Acesse no navegador:
   ```
   http://localhost:3000
   ```

## Pipeline de CI

- `.github/workflows/ci.yml` roda testes, lint e build em cada push na branch `dev`.  
- Merge em `main` dispara deploy automático (precisa configurar Secrets).
