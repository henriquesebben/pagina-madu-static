# Página MADU — versão estática

Landing page da nutricionista **Maria Eduarda Leite** em HTML + CSS puro.
Sem framework, sem build, sem Node. Feita para **GitHub Pages**.

```
index.html      estrutura + todos os textos
style.css       estilos (mobile-first; breakpoints 640 / 768 / 1024px)
assets/foto.jpg foto do hero (placeholder — trocar pela real, ~840×1000px)
assets/favicon.ico
.nojekyll        impede o GitHub de processar o site com Jekyll
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

## Publicar no GitHub Pages

1. Crie um repositório no GitHub e envie estes arquivos:
   ```bash
   git remote add origin https://github.com/SEU-USUARIO/pagina-madu.git
   git push -u origin main
   ```
2. No repositório: **Settings → Pages**.
3. **Source:** *Deploy from a branch* → branch `main` → pasta `/ (root)` → *Save*.
4. Em ~1 min o site fica em `https://SEU-USUARIO.github.io/pagina-madu/`.

Cada `git push` novo republica automaticamente. Nenhuma Action necessária.

## Antes de divulgar

- Trocar a foto placeholder.
- Preencher o número do CRN (hoje `00000`) no `index.html`.
