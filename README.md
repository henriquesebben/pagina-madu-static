# Página MADU — versão estática

Landing page da nutricionista **Maria Eduarda Leite** em HTML + CSS puro.
Sem framework, sem build, sem Node.

```
index.html      estrutura + todos os textos
style.css       estilos (mobile-first; breakpoints 640 / 768 / 1024px)
assets/foto.jpg foto do hero
assets/favicon.ico
```

## Ver localmente

Abra o `index.html` no navegador (duplo clique), ou sirva a pasta:

```bash
python3 -m http.server 8000    # depois abra http://localhost:8000
```

## Editar

- **Textos:** direto no `index.html`.
- **Cores / espaçamentos / fontes:** no topo do `style.css`, bloco `:root`.
- **Foto:** substitua `assets/foto.jpg` (mantenha o nome ou ajuste o `src` no HTML).
- **Número do WhatsApp:** aparece 6× no `index.html` (`5561920042745`) — troque todas as
  ocorrências. Também é usado nas meta tags de compartilhamento (`og:*`) no `<head>`.

## Publicar

Hospedado no **Cloudflare Pages**, projeto `mariaeduardaleite`, conectado a este
repositório. Cada `git push` na branch `main` dispara um novo deploy automático
(~1 min). Site em `https://mariaeduardaleite.pages.dev`.

Acompanhar builds: painel Cloudflare → **Workers & Pages → mariaeduardaleite → Deployments**.
