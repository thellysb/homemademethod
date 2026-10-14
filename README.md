# Clone da Estrutura - Homemade Method

Este projeto contém a estrutura completa, limpa e otimizada da página **[Homemade Method](https://homemademethod.com/)**, reconstruída sem o peso e scripts de rastreamento do WordPress original (Elementor, Perfmatters, OptiMonk, plugins proprietários), permitindo que você suba em qualquer domínio novo com carregamento instantâneo.

---

## 📁 Estrutura de Arquivos

* `index.html`: Página principal completa, responsiva (Desktop/Mobile), com todas as seções, imagens em alta definição, tipografia Lato oficial, depoimentos reais e cores da marca.

---

## ⚙️ Como Personalizar

### 1. Alterar o Link do Botão (Checkout / Quiz / VSL)
Abra o arquivo `index.html` e edite a linha 58:
```javascript
// ⚙️ INSIRA AQUI O SEU LINK DE DESTINO (QUIZ, CHECKOUT OU VSL):
const TARGET_CTA_URL = "https://seu-link-aqui.com";
```
Todos os botões *"Get Started"* da página serão atualizados automaticamente para o seu novo link!

### 2. Adicionar seu Pixel do Facebook / TikTok / GTM
No cabeçalho (`<head>`) do `index.html`, entre as linhas 60 e 73, basta colar o seu código do Pixel da Meta, Google Tag Manager ou TikTok.

### 3. Alterar Logotipo ou E-mail de Suporte
* **E-mail de suporte:** procure por `hello@homemademethod.com` e troque pelo seu e-mail de contato.
* **Logo:** substitua o link em `<header>` caso queira usar sua própria logomarca.

---

## 🚀 Como Subir no Seu Novo Domínio

### Opção 1: Cloudflare Pages / Vercel / Netlify (Grátis e Ultra Rápido)
1. Crie uma conta no [Cloudflare Pages](https://pages.cloudflare.com/), [Vercel](https://vercel.com) ou [Netlify](https://netlify.com).
2. Basta arrastar e soltar a pasta `homemademethod-clone` (ou conectar ao GitHub).
3. Conecte o seu domínio próprio nas configurações de DNS.

### Opção 2: cPanel / Hostinger / Hospedagem Tradicional
1. Acesse o **Gerenciador de Arquivos** da sua hospedagem.
2. Abra a pasta `public_html` do seu novo domínio.
3. Faça o upload do arquivo `index.html`.
4. Pronto! O site já estará no ar.
