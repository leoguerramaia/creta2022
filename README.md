# Hyundai Creta Ultimate 2022

Site estático do anúncio com painel administrativo autenticado e fotos compartilhadas pelo Supabase.

## URLs

- Página pública: https://leoguerramaia.github.io/creta2022/
- Painel: https://leoguerramaia.github.io/creta2022/admin.html

## Publicação no GitHub Pages

No repositório, abra **Settings → Pages → Build and deployment** e selecione **GitHub Actions** como fonte. O workflow `.github/workflows/pages.yml` publica o site após commits na branch `main`.

## Primeiro acesso ao painel

O painel envia um link de acesso para o e-mail administrativo autorizado: `leoguerramaia@gmail.com`.

No projeto [creta2022-anuncio no Supabase](https://supabase.com/dashboard/project/vncuarterlngephzsxpk/auth/url-configuration), configure em **Authentication → URL Configuration**:

- **Site URL:** `https://leoguerramaia.github.io/creta2022/`
- **Redirect URLs:** `https://leoguerramaia.github.io/creta2022/admin.html`

Depois, abra a URL do painel e solicite o link de acesso. O link é enviado por e-mail.

As políticas de Row Level Security permitem a leitura pública do anúncio e das fotos, mas restringem edição, upload e remoção ao e-mail autorizado. O site usa somente a chave publicável do Supabase; não adicione chaves secretas ao repositório.
