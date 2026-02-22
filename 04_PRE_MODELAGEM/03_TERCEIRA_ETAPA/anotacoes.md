#%%
# Anotações do exercício

## Análise de variável

```python
genero_counts = df_categorico['GENDER'].value_counts().reset_index()
genero_counts.columns = ['GENDER', 'COUNT']

fig = px.pie(genero_counts, names='GENDER', values='COUNT', title='Distribuição de Gênero')
fig.show()
```

Em
```python
genero_counts = df_categorico['GENDER'].value_counts().reset_index()
```
1. Com `df_categorico['GENDER']` selecionamos a coluna `GENDER` do DataFrame
2. Com `.value_counts`, contamos quantas vezes o valor que está associado à coluna aparece, no caso, quantas vezes `MASCULINO` e `FEMININO` aparece;
3. COM `.reset_index()` resetamos o index

Esses valores ficam guardados na variável `genero_counts` e ele funciona como um mini dataframe.

Agora, em:
```python
genero_counts.columns = ['GENDER', 'COUNT']
```
renomeamos as colunas do mini dataframe

plt.subplot(1, 3, 1)  # 1 linha, 2 colunas, posição 1