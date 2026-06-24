# smart-bible-versions

Arquivos JSON das traduções da Bíblia em português para o app Smart Bible.

## Nome dos arquivos

Cada arquivo segue o padrão:

```text
SIGLA - Nome da Versão Bíblica.json
```

Exemplo: `NVI - Nova Versão Internacional.json`

A NVI também está embutida no app (`assets/bible/nvi.json`); no repositório ela existe para referência, mas **não** entra na lista de download remoto.

## Versões

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

## Download RAW (GitHub)

```text
https://raw.githubusercontent.com/barretogustavo/smart-bible-versions/refs/heads/main/{nome-do-arquivo}.json
```

Use o nome do arquivo com espaços codificados na URL (o app usa `download_url` da API do GitHub).
