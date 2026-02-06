# curriculo-davidnobrega

Currículo online - David Nóbrega

## Como desenvolver localmente

Dependências principais (dev): tailwindcss, postcss, autoprefixer, concurrently, live-server

1. Instalar dependências:

```bash
npm install
```

2. Gerar CSS do Tailwind (produção):

```bash
npm run build:css
```

3. Rodar ambiente de desenvolvimento (watch CSS + servidor local com recarga):

```bash
npm run dev
```

- `npm run dev` executa `tailwindcss --watch` e `live-server` em paralelo; a página abrirá em `http://127.0.0.1:3000`.

## Estrutura importante

- `index.html` — página principal (HTML estático).
- `src/styles.css` — entrada do Tailwind (contém @tailwind directives e CSS migrado).
- `dist/styles.css` — CSS gerado (linkado no `index.html`).
- `assets/` — imagens e recursos estáticos (adicione sua foto em `assets/img/img_principal.png`).

## Atualizar foto de perfil

- Substitua `assets/img/img_principal.png` por sua foto (mesmo nome) ou atualize o `src` em `index.html`.

## Publicando (GitHub Pages)

- Eu criei uma branch `gh-pages` contendo o código pronto para deploy. Para ativar o Pages:
	- Vá em `Settings` → `Pages` e selecione a source `gh-pages` branch (ou escolha `main` se preferir). O GitHub começará a gerar o site.

## Releases / tags

- Criei uma tag anotada `v1.0.0` e a empurrei para o remoto. Você pode criar releases a partir dessa tag na interface do GitHub (Repository → Releases → Draft a new release).

## Próximos passos sugeridos

- Migrar para Vite se quiser HMR completo e suporte a frameworks (Vue/Nuxt).
- Otimizar imagens e criar `srcset` para melhor performance em mobile.
- Criar workflow GitHub Actions para build e deploy automático.

---

Se quiser que eu faça qualquer uma das ações acima (por exemplo, configurar o Pages automaticamente ou criar um workflow), diga qual e eu executo.
