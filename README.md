# Processo Seletivo — King of Languages (formulário)

Formulário de candidatura para o processo seletivo de professores da King of Languages.
Redesign do formulário, com a identidade visual da King (Poppins, vermelho `#cc213a`, navy `#061f35`).

## Como funciona

Site estático — um único arquivo `index.html` (HTML + CSS + JS, sem build).
Formulário multi-etapa estilo Typeform:

1. **Intro** — apresentação das 3 etapas do processo
2. **Nome completo**
3. **E-mail**
4. **WhatsApp (com DDD)**
5. **Confirmação** — com CTA para finalizar a candidatura no WhatsApp

Recursos: barra de progresso, validação inline, navegação por teclado (Enter),
máscara de telefone, responsivo (desktop e mobile).

## Deploy na Vercel

Não precisa de configuração. É um site estático:

1. Importar este repositório na Vercel.
2. **Framework Preset:** `Other` (ou "No Framework").
3. **Build Command:** deixar vazio. **Output Directory:** `.` (raiz).
4. Deploy.

A Vercel serve o `index.html` direto.

## ⚠️ Pendente (importante)

O envio hoje **valida os dados e mostra a tela de sucesso**, mas ainda **não salva
os dados em lugar nenhum** — falta conectar a um destino (webhook do respondi,
Kommo, Google Sheets ou e-mail). Ver o `TODO` em `submit()` no `index.html`.

- Número de WhatsApp configurado: **+55 19 99597-9055** (editável em `submit()`).

## Estrutura

```
index.html        formulário completo (HTML/CSS/JS)
assets/
  logo-branco.png   logo King (versão branca)
  simbolo-branco.png coroa King (marca d'água)
  favicon.png
```
