# Dúvidas durante o exercício.

## Label encoder x One hot-encoder

### O que é Label encoder?
Label enconder transforma variáveis categóricas em números inteiros. Exemplo:

Vermelho -> 0; Azul -> 1; Amarelo -> 2

### O que é One-Hot Encoding?
Cria uma colunabinária. Exemplo:

| Cor_Azul | Cor_Vermelha | Cor_Amarela |
|---------:|-------------:|------------:|
| 0        | 1            | 0           |
| 0        | 0            | 1           |
| 1        | 0            | 0           |

## Vantagens e desvantagens

| Aspecto                    | Label Encoding | One-Hot Encoding |
|---------------------------|----------------|------------------|
| Nº de colunas             | 1              | Uma por categoria |
| Introduz ordem falsa?     | ✅ Sim         | ❌ Não            |
| Bom para modelos lineares | ❌ Não         | ✅ Sim            |
| Bom para árvores          | ⚠️ Às vezes    | ✅ Sim            |
| Cresce muito o `.csv`     | ❌ Não         | ⚠️ Pode crescer   |

