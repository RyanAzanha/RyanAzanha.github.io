# Ryan Azanha — Portfólio

Portfólio pessoal bilíngue (PT/EN) de Ryan Azanha, Analista de Pentest / Red Team com base em Gestão de Identidades e Acessos (IAM/IGA).

- Site estático: um único `index.html`, sem build e sem dependências.
- Seletor **POR | ENG** no topo; a escolha fica salva no navegador.
- Versão com foco em IAM: abra o site com `#iam` no final do endereço
  (ex.: `https://ryanazanha.github.io/#iam`).

## Rodar localmente

Abra o `index.html` no navegador, ou:

```bash
python3 -m http.server 8000
# acesse http://localhost:8000
```

## Publicar no GitHub Pages

1. Suba os arquivos para o repositório `RyanAzanha.github.io` (branch `main`).
2. No GitHub: **Settings → Pages → Source: Deploy from a branch → main / (root)**.
3. Em 1 a 2 minutos o site fica no ar em `https://ryanazanha.github.io`.

## Como editar o conteúdo

Todo o texto fica no `<script>` do final do `index.html`:

| O que mudar | Onde |
|---|---|
| Textos gerais (hero, títulos) | `DATA.pt` e `DATA.en` |
| Versão IAM do topo | `IAM.pt` e `IAM.en` |
| Fundamentos | `FUND` |
| Experiência (ordenada por `start`) | `JOBS` |
| Projetos | `PROJECTS` |
| Laboratórios | `LABS` |
| Formação | `EDU` |
| Certificações e trilha | `CERT_DONE` e `ROADMAP` |

Ao concluir uma certificação: mova-a de `ROADMAP` para `CERT_DONE` e marque a próxima como `status: "now"`.

## Domínio próprio (opcional)

Compre o domínio (ex.: `ryanazanha.com.br` no Registro.br), crie um arquivo `CNAME` na raiz com o domínio e configure o DNS conforme a documentação do GitHub Pages.
