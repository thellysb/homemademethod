# 🚀 Clone Estrutura Completa - AdEvaluator Pro & Facebook Rewards (`boardcrafted.online`)

Clone 100% funcional, independente e pronto para produção do funil completo de **Facebook Rewards / AdEvaluator Pro™**, incluindo a página principal do quiz/VSL e a página de confirmação de pedido e acesso imediato (`/thanks/`).

---

## 📁 Estrutura Completa de Arquivos

```
boardcrafted-clone/
├── index.html                                 # Página principal do Funil (Passo 0 -> Posts 1 a 3 -> VSL Final)
├── MetaTraffic_Pro_Master_Curriculum_Guide.pdf# Guia em PDF do currículo oficial (download direto)
├── contact.html                               # Página de suporte e helpdesk do cliente
├── terms.html                                 # Termos de serviço
├── privacy.html                               # Política de privacidade
├── refund.html                                # Política de reembolso e garantia de 30 dias
├── impressum.html                             # Aviso legal (compliance e transparência)
├── README.md                                  # Manual completo de configuração e deploy
│
├── thanks/
│   └── index.html                             # Página de confirmação de pedido & entrega de acesso
│
├── css/
│   └── MM3nXP63nRRs.css                       # Folha de estilo Tailwind CSS da página principal
├── fonts/
│   ├── CC4SL5HrrGCk.woff2                     # Fonte Red Hat Display local
│   └── nnlQyFX0dpT2.woff2                     # Fonte Red Hat Display local
├── images/
│   ├── DF32jO8vZckV.png                       # Favicon oficial
│   ├── Facebook_Logo_(2019).svg               # Logo do Facebook no cabeçalho
│   ├── verified.png                           # Selo azul de verificado
│   ├── bMLFkPEGl3xh.webp                      # Foto de perfil Mark Zuckerberg
│   ├── Yl8jFpPF17D9.png                       # Foto do usuário
│   ├── amazon_logo.webp                       # Logo da Amazon
│   ├── amazon_post.webp                       # Foto do post da Amazon
│   ├── apple_logo.webp                        # Logo da Apple
│   ├── apple_post.webp                        # Foto do post da Apple
│   ├── starbucks_logo.webp                    # Logo da Starbucks
│   ├── starbucks_post.webp                    # Foto do post da Starbucks
│   └── avatars/                               # 16 avatares dos comentários e do chat salvos localmente
└── js/
    ├── BDTxNxyJpnED.js                        # Script de tracking Utmify
    ├── wAFZJQpKHWNK.js                        # Script de preservação e repasse de UTMs
    └── twemoji.min.js                         # Biblioteca Twemoji local
```

---

## ⚙️ Painel de Configurações (Fácil Edição)

No topo do arquivo [`index.html`](file:///C:/Users/GAMER%20-%20PC/.gemini/antigravity/scratch/boardcrafted-clone/index.html) (linhas 20 a 35), há um painel centralizado para configurar seus IDs de rastreamento e seu vídeo Vturb:

```html
<script>
  window.APP_CONFIG = {
    // 1. ID do Pixel do Facebook (substitua pelo seu ID numérico):
    facebookPixelId: "841455795723124",

    // 2. ID do Pixel UTMify (substitua pelo seu ID alfanumérico):
    utmifyPixelId: "6a8fa5e28f2a32233dd4463c",

    // 3. Configuração do Vídeo Vturb / ConverteAI:
    vturb: {
      playerId: "vid-6ad7f13ce661f216ee2e23ce",
      playerScript: "https://scripts.converteai.net/f37349c9-5d96-4c50-baa3-6990edef6733/players/6ad7f13ce661f216ee2e23ce/v4/player.js"
    }
  };
</script>
```

Na página de obrigado ([`thanks/index.html`](file:///C:/Users/GAMER%20-%20PC/.gemini/antigravity/scratch/boardcrafted-clone/thanks/index.html)), o Pixel da Utmify e o preservador automático de UTMs já estão devidamente integrados.

---

## 🌐 Como Subir no Seu Novo Domínio

Você pode subir toda a estrutura facilmente em qualquer provedor de hospedagem:

### Opção 1: cPanel / Hostinger / Apache / Nginx
1. Acesse o Gerenciador de Arquivos da sua hospedagem.
2. Vá até a pasta raiz do seu domínio (geralmente `public_html/`).
3. Envie todos os arquivos e pastas da pasta `boardcrafted-clone`:
   - `index.html`
   - `contact.html`, `terms.html`, `privacy.html`, `refund.html`, `impressum.html`
   - `MetaTraffic_Pro_Master_Curriculum_Guide.pdf`
   - Pasta `thanks/` (com seu `index.html`)
   - Pastas `css/`, `fonts/`, `images/`, `js/`
4. Acesse:
   - Funil Principal: `https://seunovodominio.com/`
   - Página de Obrigado: `https://seunovodominio.com/thanks/`

### Opção 2: Vercel / Netlify / Cloudflare Pages
1. Arraste ou importe a pasta `boardcrafted-clone` para o painel da Vercel / Netlify.
2. Não precisa de build command, o deploy é instantâneo e estático.

---

## 🔄 Fluxo e Funcionalidades

1. **Página de Entrada (`/`)**:
   - Card de boas-vindas com saldo inicial de **US$ 32.27**.
   - 3 passos de avaliação interativa (Amazon, Apple, Starbucks) acumulando saldo até **US$ 278.45**.
   - VSL com player Vturb integrado, comentários sociais em tempo real e repasse automático de UTMs para o checkout.
2. **Página de Confirmação (`/thanks/`)**:
   - Confirmação oficial de pagamento e garantia de 30 dias.
   - Orientações detalhadas de recebimento por e-mail e Google Drive.
   - Central de Acesso com download direto do PDF do currículo e links de acesso aos upgrades (UP1 a UP4).
   - Links funcionais de suporte, termos, privacidade e reembolso.
