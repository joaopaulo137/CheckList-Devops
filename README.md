# Checklist-Devops

### ✅ Checklist DevOps – GitHub Actions

### 🔒 1. Bloquear commits diretos na `main`

🎯 Objetivo
Garantir que ninguém faça push direto — tudo deve passar por PR.

### 🔁 2. Exigir aprovação de PR para merge

🎯 Objetivo
Implementar fluxo correto de revisão.

✅ O que fazer
Já dentro da rule criada:

🚫 Require pull request reviews before merging

Definir: 1 ou mais aprovadores

### ⚙️ 3. Criar e usar GitHub Actions

🎯 Objetivo: Criar pipelines automáticos.

### ♻️ 4. Reaproveitar Actions do marketplace

🎯 Objetivo: Evitar reinventar roda.

💡 Exercício
Montar pipeline que: Instala dependências; Roda teste.

### 🔐 5. Trabalhar com Secrets
🎯 Objetivo:
Proteger dados sensíveis (tokens, senhas, etc.)

✅ Criar secret

✅ Usar no workflow

### ⚠️ Importante
Nunca dar `echo` em produção (vaza segredo nos logs)
Usar apenas quando necessário

### 📦 6. Upload de arquivos (Artifacts)
🎯 Objetivo: Salvar resultados do build/testes

### 7. Combinar tudo
🎯 Objetivos:

✅ Rodar em PR

✅ Bloquear merge se pipeline falhar

✅ Usar pelo menos 1 action do marketplace

✅ Usar 1 secret

✅ Gerar e subir artifact

### 8. Criar pipeline com environment para deploy com permissão do reviwer
🎯 Objetivos:

✅ Rodar o build

✅ Definir o environment

✅ Aprovar a execução do pipeline

✅ Executar deploy
