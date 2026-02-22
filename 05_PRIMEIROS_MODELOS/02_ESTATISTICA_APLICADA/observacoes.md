## `np.mean(x)` vs `x.mean()`

- `np.mean(x)` é uma função do NumPy e aceita qualquer objeto *array-like*
  (listas, tuplas, `ndarray`).
- `x.mean()` é um método do `numpy.ndarray` e só funciona se `x` for um array NumPy.
- Para `ndarray`, ambos produzem o mesmo resultado, pois `np.mean(x)` chama
  internamente `x.mean()`.
- Diferenças podem aparecer apenas em subclasses de `ndarray`.

**Regra prática:**  
Use `np.mean(x)` quando o tipo for incerto;  
use `x.mean()` quando souber que é um `ndarray`.
