# HabitPAY — Landing Page (Link in Bio)

Página única ("link in bio") com a identidade visual da HabitPAY, reunindo todos os canais oficiais e links de produto em um só lugar.

## Sobre a HabitPAY

**HabitPAY** é uma fintech e startup brasileira focada em inteligência financeira e no desenvolvimento de hábitos monetários saudáveis. A proposta vai além do controle financeiro: o objetivo é transformar a relação das pessoas com o dinheiro por meio de consistência e inteligência.

Sediada no sudoeste do Paraná, com forte atuação regional, a empresa vem se destacando no cenário nacional — foi selecionada para o **Founders Club Growth Challenge**, ficando entre as melhores startups do país.

| | |
|---|---|
| **Razão social / Marca** | HabitPAY |
| **CNPJ** | 66.877.250/0001-12 |
| **Endereço** | R. Pedro Álvares Cabral, 905 — Centro Norte, Dois Vizinhos - PR, 85660-000 |

## Preview

A página inclui:

- **Hero** com logo, tagline oficial e selo de destaque (Founders Club Growth Challenge)
- **Comece por aqui** — Lista de Espera (CTA principal) e HabitPAY Insights
- **Redes sociais** — Instagram, LinkedIn, YouTube e Canal do WhatsApp
- **Sobre a HabitPAY** — bloco institucional resumido
- **Rodapé** com CNPJ e endereço

## Links inclusos

| Canal | Link |
|---|---|
| Lista de Espera | https://habitpay.vercel.app/ |
| HabitPAY Insights | https://habit-pay-insights.vercel.app/ |
| Instagram | https://www.instagram.com/habitpay.app/ |
| LinkedIn | https://www.linkedin.com/company/apphabitpay |
| YouTube | https://www.youtube.com/@habitpay |
| Canal do WhatsApp | https://www.whatsapp.com/channel/0029Vb7Hb1f7YSd9O2xMRa2N |

## Stack

Página estática em **HTML + CSS puro** (vanilla), sem dependências de build ou frameworks. A logo é embutida como Base64 diretamente no HTML, então o arquivo funciona sozinho — basta abrir no navegador.

- Tipografia: [Sora](https://fonts.google.com/specimen/Sora) (display) + [Inter](https://fonts.google.com/specimen/Inter) (corpo), via Google Fonts
- Sem JavaScript de terceiros, sem analytics, sem cookies
- Responsivo (mobile-first) e com `prefers-reduced-motion` respeitado

## Estrutura

```
.
├── index.html      # página completa (HTML + CSS + logo em base64)
└── README.md
```

## Como rodar localmente

Não há build nem dependências. Basta abrir o arquivo direto no navegador:

```bash
open index.html        # macOS
xdg-open index.html    # Linux
start index.html       # Windows
```

Ou suba um servidor estático simples para testar com live reload básico:

```bash
python3 -m http.server 8000
# acesse http://localhost:8000
```

## Deploy

Por ser um único arquivo HTML estático, pode ser publicado em qualquer serviço de hospedagem estática:

- **Vercel**: `vercel deploy` na raiz do projeto
- **Netlify**: arraste a pasta no [app.netlify.com/drop](https://app.netlify.com/drop)
- **GitHub Pages**: ative em *Settings → Pages*, apontando para a branch/diretório raiz

## Personalização

Os tokens de cor e tipografia ficam no `:root` do `index.html`:

```css
:root{
  --navy-deep: #0c1730;   /* fundo principal */
  --navy: #14223f;
  --navy-soft: #1c2c4d;   /* fundo dos cards */
  --blue: #2196d8;        /* azul HabitPAY */
  --blue-bright: #38b6ff;
  --green: #4ade80;       /* verde do logo */
  --green-deep: #22c55e;
  --ink: #f6f8fc;         /* texto principal */
  --ink-dim: #aab4c8;     /* texto secundário */
}
```

Para adicionar ou editar um link, duplique um bloco `.link-card` dentro da seção desejada em `index.html`.

## Licença

Uso interno — HabitPAY. Todos os direitos reservados.
