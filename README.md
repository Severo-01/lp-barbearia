# Barbearia — Landing page

Site estático hospedado na Vercel.

## Estrutura

- `index.html` — landing page
- `vercel.json` — cabeçalhos de segurança (CSP com hashes, HSTS, etc.)
- `/fornecedor/` — GSAP e ScrollTrigger hospedados localmente
- `scripts/gerar-csp.py` — regenera o `vercel.json` (rodar após mudar qualquer script do `index.html`)
