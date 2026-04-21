# CLAUDE.md

Instruções para Claude Code trabalhando neste repositório.

## Sobre o projeto

Repositório de estudos da linguagem **Go** — exemplos, exercícios e notas de aulas. Cada diretório/arquivo tende a ser autocontido (foco didático, não produção).

## Stack

- Linguagem: **Go** (1.26+)
- Ferramentas: `go`, `go test`, `go vet`, `gofmt`
- Sem framework web padrão — varia por exemplo

## Convenções

- Código idiomático Go: seguir `gofmt` e `go vet`.
- Nomes em inglês no código; comentários e notas didáticas podem ficar em português.
- Preferir exemplos minimalistas e autoexplicativos (este é um repo de aprendizado).
- Cada tópico/aula em seu próprio diretório quando fizer sentido (ex.: `01-basics/`, `02-goroutines/`).
- `go.mod` por diretório só quando necessário; caso contrário, um módulo único na raiz.

## Comandos úteis

```bash
go run ./caminho        # rodar um exemplo
go test ./...           # rodar todos os testes
go vet ./...            # análise estática
gofmt -w .              # formatar tudo
go mod tidy             # limpar dependências
```

## Diretrizes para o assistente

- **Não criar arquivos de documentação** (`README.md`, notas, planos) sem pedido explícito.
- **Preferir editar** arquivos existentes a criar novos.
- Não adicionar abstrações ou tratamento de erro defensivo desnecessário — o foco é didático.
- Comentários só quando o "porquê" não é óbvio.
- Antes de ações destrutivas (delete, reset, force-push), pedir confirmação.
- Commits seguem **Conventional Commits** (`feat:`, `fix:`, `docs:`, etc.) e só são criados quando solicitados.
