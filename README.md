# smart-bible-versions

Arquivos JSON das traduções da Bíblia para o app Smart Bible, organizados por idioma.

## Estrutura

```text
smart-bible-versions/
  portuguese/
    SIGLA - Nome da Versão Bíblica.json
    ...
  english/
    SIGLA - Version Name.json
    ...
```

## Nome dos arquivos

Cada arquivo, em qualquer pasta, segue o padrão:

```text
SIGLA - Nome da Versão Bíblica.json
```

Exemplo (PT): `NVI - Nova Versão Internacional.json`
Exemplo (EN): `NIV - New International Version.json`

A sigla antes do ` - ` é usada pelo app como identificador interno da versão (`versionId`), em minúsculas.

A NVI (PT) e a NIV (EN) também estão embutidas no app (`assets/bible/nvi.json` e `assets/bible/niv.json`); nos repositórios elas existem para referência, mas **não** entram na lista de download remoto.

## Versões — Português (`portuguese/`)

| Sigla | Nome |
|-------|------|
| ACF | Almeida Corrigida e Fiel |
| ARA | Almeida Revista e Atualizada |
| ARC | Almeida Revista e Corrigida |
| AS21 | Almeida Século 21 |
| JFAA | Almeida Atualizada |
| KJA | King James Atualizada |
| KJF | King James Fiel |
| NAA | Nova Almeida Atualizada |
| NBV | Nova Bíblia Viva |
| NTLH | Nova Tradução na Linguagem de Hoje |
| NVI | Nova Versão Internacional |
| NVT | Nova Versão Transformadora |
| TB | Tradução Brasileira |
| BLIVRE | Bíblia Livre |
| ALM1911 | Almeida 1911 |
| OL | O Livro |
| MENS | A Mensagem |
| VFL | Versão Fácil de Ler |

## Versões — English (`english/`)

| Sigla | Nome |
|-------|------|
| NIV | New International Version |
| KJV | King James Version |
| NKJV | New King James Version |
| ESV | English Standard Version |
| KJVA | King James Version with Apocrypha |
| KJVCPB | King James Version Cambridge Paragraph Bible |

> **Nota de licenciamento:** a NIV não é de domínio público; distribuí-la embutida no app (`assets/bible/niv.json`) requer licença da Biblica. Confirme os direitos de uso antes de publicar o app internacionalmente com a NIV como versão padrão.

## Download RAW (GitHub)

```text
https://raw.githubusercontent.com/barretogustavo/smart-bible-versions/refs/heads/main/portuguese/{nome-do-arquivo}.json
https://raw.githubusercontent.com/barretogustavo/smart-bible-versions/refs/heads/main/english/{nome-do-arquivo}.json
```

Use o nome do arquivo com espaços codificados na URL (o app usa `download_url` da API do GitHub).

## Listagem via API (GitHub)

```text
https://api.github.com/repos/barretogustavo/smart-bible-versions/contents/portuguese?ref=main
https://api.github.com/repos/barretogustavo/smart-bible-versions/contents/english?ref=main
```

O app consulta o endpoint correspondente ao idioma selecionado para montar o catálogo de versões disponíveis para download.
