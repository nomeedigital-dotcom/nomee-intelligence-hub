# NOMEE INTELLIGENCE HUB

**Plataforma de Diagnóstico Empresarial, Organização de Clientes e Relatórios PDF (Método NOMEE EDGE)**

Aplicação web enxuta, responsiva e sem backend pago, construída em arquivo único (`index.html`) para hospedagem gratuita no **GitHub Pages** com banco de dados em tempo real no **Supabase (Plano Gratuito)**.

---

## 1. Estrutura Oficial do Repositório

Suba **apenas estes 5 arquivos** para o seu repositório no GitHub:

```text
nomee-intelligence-hub/
├── index.html            # Aplicação completa (Landing + Portal Cliente + Formulário 7 Etapas + Power BI + PDF)
├── supabase_schema.sql   # Script SQL para criar a tabela public.nomee_clients no Supabase
├── README.md             # Documentação do projeto
├── DEPLOY_GITHUB.md      # Passo a passo de publicação no Supabase + GitHub Pages
└── .gitignore            # Proteção contra versionamento de chaves locais e backups
```

---

## 2. O que a Plataforma Entrega

* **Landing Page + Área de Acesso Segura:** Visual corporativo escuro (*Obsidian & Blood Red*), login com e-mail e PIN e modo exclusivo para clientes via URL travada (`?portal=cliente&c=NOM-0001`).
* **Portal do Cliente + Gráficos Prévios:** Antes mesmo de baixar o PDF, o cliente visualiza o **Mapa de Maturidade dos 7 Módulos** e a **Qualidade das Informações** diretamente na tela.
* **Formulário Estruturado (7 Módulos):** Salvamento automático em tempo real direto no **Supabase**, opção *"Não sei"* sem bloqueio, registro de anexos e Termo **LGPD (retenção de 24 meses)** com protocolo único (`PRT-2026-XXXX`).
* **Dashboard Estilo Power BI (`Chart.js`):** Segmentadores dinâmicos (*Empresa, Segmento, Status, Liberação PDF e Busca*) e 4 gráficos interativos com filtro cruzado ao clicar.
* **Pastas Padronizadas:** Organização automática no formato **`Nome do Cliente - Nome da Empresa`** com exclusão segura e geração de link exclusivo do portal.
* **Relatório Oficial em PDF (`jsPDF` A4):** Pré-visualização completa na tela e download direto em PDF vetorial formatado, destacando automaticamente os campos ausentes ou marcados como *"Não sei"* para validação.

---

## 3. Credenciais Padrão de Teste

* **Diretoria (Admin):** `admin@nomee.company` — PIN: `990011`
* **Cliente de Exemplo:** `cliente@vertice.com.br` — PIN: `123456`

> **Segurança:** O arquivo `index.html` utiliza exclusivamente a **URL do projeto** e a **Publishable Key** do Supabase. Nunca coloque sua `service_role` / `secret key` em repositórios públicos.