# PIX DO MILHÃO · Combo dos Sonhos

Landing page estática para a oferta "Combo dos Sonhos" da PIX DO MILHÃO (250 chances por R$29,90 · 90% off).

## Stack
- HTML único + CSS puro + JS vanilla
- Google Fonts (Ubuntu)
- Hospedagem: GitHub Pages

## Estrutura
```
.
├── index.html        # Página completa (HTML + CSS + JS inline)
├── assets/           # Imagens exportadas do Figma
└── README.md
```

## Origem do design
Figma: [Pop-Up VIP · MOBILE1](https://www.figma.com/design/RnKHrLVXX1yr5CagDU1qLl/Pop-Up-VIP?node-id=68-1055)

## Componentes interativos
- **Stepper de quantidade**: chips +10/+20/+50, input com -/+, preço calculado em tempo real (R$1,99/chance)
- **Timer da barra**: countdown de 2h persistido em localStorage (`pdm_offer_end`)
- **Marquee**: scroll horizontal contínuo (CSS animation)
- **Fade-in**: elementos com `.fade-in` revelam ao entrar na viewport (IntersectionObserver)

## Checkout
Os botões `[data-checkout]` estão como placeholder. Substituir o `window.location.href` no final do `<script>` por:
- URL real da Greenn / plataforma de pagamento
- Webhook para tracking (UTMs, fbp, fbc) se aplicável

## Deploy
Repo: [github.com/hxcorp2025/pdm_pages](https://github.com/hxcorp2025/pdm_pages)
Live: ativar GitHub Pages em Settings → Pages → branch `main` / pasta `/`.
