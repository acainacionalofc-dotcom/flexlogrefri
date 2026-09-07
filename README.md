# FlexLog — site institucional

Site estático (HTML/CSS/JS puro, sem build) pronto para publicar na Vercel.

## Estrutura
```
index.html      → site completo (todas as seções + rastreamento)
assets/logo.png → logomarca FlexLog
vercel.json     → configuração mínima (URLs limpas)
```

## Como publicar na Vercel

**Opção 1 — Vercel CLI**
```bash
npm i -g vercel
cd flexlog
vercel        # ambiente de preview
vercel --prod # publica em produção
```

**Opção 2 — Painel da Vercel**
1. Suba esta pasta para um repositório no GitHub/GitLab/Bitbucket.
2. Em vercel.com → "Add New Project" → importe o repositório.
3. Framework Preset: **Other** (site estático). Não é necessário comando de build nem diretório de saída.
4. Deploy.

**Opção 3 — Arrastar e soltar**
Em vercel.com, use "Deploy" → arraste a pasta `flexlog` (com `index.html` e `assets/`) diretamente.

## Rastreamento (simulado)
- Único código válido: `BR35318887` → exibe status **Emitindo a nota fiscal**, origem **Vila Liviero — São Paulo/SP**, com timeline (somente a 1ª etapa ativa).
- Qualquer outro código → mensagem de erro.
- Toda a lógica roda no navegador (JavaScript), sem backend nem banco de dados.

## Personalização
- Cores e tipografia: variáveis CSS no topo do `<style>` em `index.html` (`--navy-900`, `--cyan-500` etc.).
- Textos de contato (telefone/e-mail/endereço) não foram inventados — adicione-os no rodapé e na seção de contato quando tiver essas informações.
