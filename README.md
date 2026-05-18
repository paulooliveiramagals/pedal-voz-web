# pedal-voz-web

Pedal virtual de voz profissional para navegador, com visual escuro estilo SaaS/pedal físico, feito em **HTML + Tailwind CSS + JavaScript puro**.

## Funcionalidades
- Entrada de microfone
- Reverb (mix/decay)
- Delay (time/feedback)
- EQ 3 bandas (grave/médio/agudo)
- Compressor simples (threshold/ratio)
- Botão de bypass
- VU meter em tempo real

---

## Como visualizar o projeto funcionando (local)

### 1) Clonar e entrar no projeto
```bash
git clone https://github.com/SEU_USUARIO/pedal-voz-web.git
cd pedal-voz-web
```

### 2) Subir um servidor local simples
> Recomendado para evitar bloqueios de mídia/permissão do navegador.

```bash
python3 -m http.server 5500
```

### 3) Abrir no navegador
Acesse:

```text
http://localhost:5500/index.html
```

### 4) Ativar áudio
- Clique em **Ativar Microfone**
- Permita o acesso ao microfone
- Ajuste os controles
- Use **Bypass** para comparar áudio seco/processado

---

## Publicar no GitHub Pages (jeito simples)

Este repositório já inclui um workflow de deploy automático. Basta:

1. Subir o código para o GitHub.
2. No GitHub, vá em **Settings → Pages**.
3. Em **Build and deployment**, selecione **Source: GitHub Actions**.
4. Faça push na branch `main` (ou execute o workflow manualmente).
5. Aguarde o workflow **Deploy static site to GitHub Pages** finalizar.
6. Seu site ficará em:

```text
https://SEU_USUARIO.github.io/pedal-voz-web/
```

---

## Estrutura
```text
.
├── index.html
├── README.md
└── .github/
    └── workflows/
        └── deploy-pages.yml
```
