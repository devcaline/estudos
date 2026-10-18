# Tema B2 — Chamadas de Emergência

Projeto da **AV3** de Estrutura de Dados — UNIJORGE, Turma A.

**Responsável:** William Silva Lago

## Descrição

Programa de console em C que gerencia **chamadas de emergência** usando uma
**pilha**: a última chamada registrada é a primeira a ser atendida. Os dados
podem ser salvos e carregados de um arquivo CSV, e o relatório pode ser
exportado em TXT.

## Funcionalidades

- Registrar chamada (push)
- Atender chamada (pop)
- Consultar última chamada (peek)
- Listar todas as chamadas
- Salvar dados em CSV
- Carregar dados de CSV
- Gerar relatório de chamadas
- Exportar relatório em TXT
- Limpar pilha com confirmação
- Validação de horário (HH:MM)
- Controle automático de protocolo

## Menu do sistema

```text
1 - Registrar chamada
2 - Atender chamada
3 - Consultar última chamada
4 - Listar chamadas
5 - Salvar CSV
6 - Carregar CSV
7 - Gerar relatório
8 - Exportar relatório TXT
9 - Limpar pilha
0 - Sair
```

## Como compilar e executar

Pré-requisito: ter o compilador **gcc** instalado.

Dentro desta pasta (`chamadas-de-emergencia/`):

```bash
# Compilar
gcc -std=c99 -Wall -pedantic main.c -o chamadas

# Executar
./chamadas
```

No Windows (com MinGW), o executável é `chamadas.exe`:

```bash
gcc -std=c99 -Wall -pedantic main.c -o chamadas.exe
chamadas.exe
```

## Arquivos

- [`main.c`](main.c) — código-fonte completo do programa.
- [`chamadas.csv`](chamadas.csv) — arquivo de persistência das chamadas (gerado/lido pelo programa).
- [`relatorio.txt`](relatorio.txt) — exemplo de relatório exportado pelo programa.
