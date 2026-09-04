# CRUD de Carros em Python

Projeto desenvolvido como exercício de estudo em Python, com o objetivo de praticar operações básicas de CRUD em memória.

## Funcionalidades

O sistema permite:

- Cadastrar carros
- Listar carros cadastrados
- Buscar carros pela placa
- Editar informações de um carro
- Deletar carros
- Validar placas duplicadas
- Manter valores atuais durante a edição ao pressionar Enter

## Estrutura dos dados

Os carros são armazenados em uma lista de dicionários.

Exemplo:

```python
carro = {
    "placa": "ABC-1234",
    "cor": "Preto",
    "modelo": "Onix",
    "ano": 2022
}
```

## Conceitos praticados

Durante o desenvolvimento deste projeto, pratiquei:

- Funções
- Parâmetros e retorno com `return`
- Listas
- Dicionários
- Lista de dicionários
- Estruturas condicionais (`if`, `elif`, `else`)
- Laços de repetição (`for` e `while`)
- `break`
- `None`
- Manipulação de strings com `strip()` e `lower()`
- Uso de `len()`
- Conversão de tipos com `int()`
- Tratamento de erros com `try` e `except`
- Reutilização de funções

## Funcionamento

Ao cadastrar um carro, o sistema solicita placa, cor, modelo e ano e armazena essas informações em um dicionário dentro da lista de carros.

A função `encontrar_carro()` percorre a lista e procura um veículo pela placa. Essa função é reutilizada nas operações de edição e exclusão.

Ao editar um carro, o sistema permite alterar apenas os campos desejados. Caso o usuário pressione Enter sem digitar um novo valor, o dado atual é mantido.

Antes de alterar uma placa, o sistema verifica se já existe outro carro cadastrado com a mesma placa.

Ao deletar um carro, o sistema procura o veículo pela placa e, caso ele exista, remove o dicionário correspondente da lista.

## Como executar

Clone o repositório:

```bash
git clone URL_DO_REPOSITORIO
```

Entre na pasta do projeto:

```bash
cd projeto-crud-carros
```

Execute o programa:

```bash
python3 codigo.py
```

## Objetivo do projeto

Este projeto faz parte dos meus estudos de fundamentos de Python e foi desenvolvido para consolidar conceitos de lógica de programação, funções, listas, dicionários, validações e tratamento de erros antes de avançar para aplicações com APIs e bancos de dados.
