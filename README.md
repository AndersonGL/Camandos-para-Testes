# Camandos-para-Testes


# 🧪 Testes Automatizados em Next.js

Este projeto utiliza diferentes estratégias de testes para garantir qualidade, confiabilidade e estabilidade da aplicação.

---

## 📌 1. Testes de Componentes e Unidade  
**(Jest + React Testing Library)**

Estes testes validam componentes individuais da interface (UI) e funções isoladamente.

### ▶️ Executar testes

```bash
npm test
# ou
yarn test
```

Executa os testes Jest uma única vez.

---

### 👀 Modo Watch (monitoramento automático)

```bash
npm test -- --watch
# ou
jest --watch
```

Monitora alterações nos arquivos e reexecuta os testes automaticamente.

---

### 📊 Gerar relatório de cobertura

```bash
npm test -- --coverage
# ou
jest --coverage
```

Executa os testes e gera relatório de cobertura de código.

---

### 🔄 Modo Interativo (watchAll)

```bash
npm test -- --watchAll
```

Executa todos os testes em modo interativo.

---

## 🌐 2. Testes Automatizados de UI / E2E  
### (Cypress)

O Cypress simula o comportamento real do usuário no navegador para testes End-to-End.

### 🖥 Abrir interface gráfica

```bash
npx cypress open
# ou
npm run cypress:open
```

---

### ⚙️ Executar em modo headless (ideal para CI/CD)

```bash
npx cypress run
# ou
npm run cypress:run
```

---

## 🎭 3. Testes Automatizados de UI / E2E  
### (Playwright)

O Playwright é uma alternativa moderna e rápida para automação de testes E2E.

### ▶️ Executar todos os testes

```bash
npx playwright test
```

---

### 🖥 Abrir interface gráfica

```bash
npx playwright test --ui
```

---

### 🌍 Executar em navegador específico (Chromium)

```bash
npx playwright test --project=chromium
```

---

## ⚙️ 4. Outros Comandos Importantes

### 🏗 Build do projeto

```bash
npm run build
```

Garante que o projeto compile sem erros antes da execução de testes E2E.

---

### 🧹 Lint (Análise estática de código)

```bash
next lint
```

Executa o ESLint para verificar padrões e qualidade do código.

---

## 📦 Exemplo de Configuração no `package.json`

```json
{
  "scripts": {
    "dev": "next dev",
    "build": "next build",
    "start": "next start",
    "test": "jest",
    "test:watch": "jest --watch",
    "cypress:open": "cypress open",
    "cypress:run": "cypress run"
  }
}
```

---

## ✅ Estratégia de Testes Utilizada

- ✔ Testes Unitários → Funções isoladas  
- ✔ Testes de Componentes → Interface individual  
- ✔ Testes E2E → Fluxo completo do usuário  
- ✔ Lint + Build → Qualidade e integridade do projeto  

---

## 🚀 Objetivo

Garantir:

- Qualidade de código  
- Confiabilidade em produção  
- Segurança em deploys  
- Integração contínua (CI/CD) eficiente  

---

Feito com foco em qualidade, automação e boas práticas 💻✨
