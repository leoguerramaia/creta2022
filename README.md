# Hyundai Creta Ultimate 2022

Site estático do anúncio com painel administrativo autenticado e fotos compartilhadas pelo Supabase.

## URLs após a publicação

- Página pública: https://leoguerramaia.github.io/creta2022/
- Painel: https://leoguerramaia.github.io/creta2022/admin.html

## Publicar pelo GitHub Pages

Este repositório precisa estar **público** para usar GitHub Pages no plano atual. Tornar o repositório público também torna os arquivos do projeto visíveis a qualquer pessoa.

1. Abra **Settings → General → Danger Zone → Change repository visibility** e altere para **Public**.
2. Abra **Settings → Pages → Build and deployment** e escolha **GitHub Actions** como fonte.
3. O workflow `.github/workflows/pages.yml` fará o deploy após um novo commit na branch `main`. Se necessário, execute-o em **Actions → Deploy Creta site to GitHub Pages → Run workflow**.

## Primeiro acesso ao painel

O painel envia um link de acesso para o e-mail administrativo autorizado: `leoguerramaia@gmail.com`.

No projeto [creta2022-anuncio no Supabase](https://supabase.com/dashboard/project/vncuarterlngephzsxpk/auth/url-configuration), configure em **Authentication → URL Configuration**:

- **Site URL:** `https://leoguerramaia.github.io/creta2022/`
- **Redirect URLs:** `https://leoguerramaia.github.io/creta2022/admin.html`

Depois, abra a URL do painel e solicite o link de acesso. O link é enviado por e-mail.

As políticas de Row Level Security permitem leitura pública do anúncio e das fotos, mas restringem edição, upload e remoção ao e-mail autorizado. O site usa somente a chave publicável do Supabase; não adicione chaves secretas ao repositório.
