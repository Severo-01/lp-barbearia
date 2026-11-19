Barbearia — Página de destino

Landing page estática da barbearia, hospedada na Vercel.

Estrutura do projeto
text
/
├── index.html
├── vercel.json
├── README.md
├── .gitignore
├── .vercelignore
├── fornecedor/
│   ├── gsap.min.js
│   └── ScrollTrigger.min.js
└── scripts/
    └── gerar-csp.py

Arquivos principais
index.html — página principal (landing page).
vercel.json — configuração dos cabeçalhos de segurança, incluindo CSP com hashes SHA-256, HSTS e outras proteções.
fornecedor/ — bibliotecas GSAP e ScrollTrigger hospedadas localmente, sem dependência de CDNs externos.
scripts/gerar-csp.py — script para regenerar os hashes da CSP e atualizar o vercel.json.
Segurança
Content Security Policy (CSP) com hashes SHA-256.
HSTS.
X-Content-Type-Options.
X-Frame-Options.
Referrer-Policy.
Permissions-Policy.
Bibliotecas JavaScript hospedadas localmente.
Manutenção

Sempre que houver alterações nos scripts JavaScript incorporados ao index.html, execute:

bash
python3 scripts/gerar-csp.py


Isso atualiza os hashes utilizados pela CSP no vercel.json.

Hospedagem

Projeto estático hospedado na Vercel, com integração ao GitHub para controle de versões e deploy automático.
