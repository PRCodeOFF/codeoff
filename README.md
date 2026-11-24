# codeoff.com.br

Site estático servido pela Vercel. Sem build, sem dependências.

| Rota | Arquivo |
|---|---|
| `/` | `index.html` |
| `/privacy` | `privacy/index.html` |

`/privacidade`, `/politica-de-privacidade` e `/privacy-policy` redirecionam (301) para `/privacy`.

## Deploy

1. `git push` para `main` — a Vercel publica automaticamente.
2. No projeto da Vercel: **Framework Preset = Other**, sem build command e output `.` (raiz).
3. Em **Settings → Domains**, adicionar `codeoff.com.br` e `www.codeoff.com.br`.

Pré-visualizar localmente: `npx serve .` e abrir `http://localhost:3000/privacy`.

## Antes de publicar na Google Play

- [ ] Preencher razão social e CNPJ na seção 1 da política
- [ ] Criar as caixas `privacidade@` e `dpo@` em codeoff.com.br
- [ ] Conferir se as seções 3, 6 e 7 batem com o que cada app realmente coleta
- [ ] Ajustar o caminho de exclusão no app (seção 11) para o fluxo real
- [ ] Colar `https://codeoff.com.br/privacy` no Play Console em **Política > Conteúdo do app > Política de Privacidade**
- [ ] Mesma URL no formulário de **Exclusão de dados** do Play Console
