# 🏠 Regressão Linear Múltipla – Prevendo Preços de Imóveis na Califórnia

Este projeto demonstra como aplicar uma **regressão linear múltipla** usando Python para prever o preço de imóveis na Califórnia com base em diversas variáveis explicativas. O objetivo é entender como diferentes fatores influenciam o valor final de uma propriedade.

---

## 📁 Sobre o Dataset

O conjunto de dados contém diversas colunas com informações sobre regiões da Califórnia. A variável que queremos prever é:

- `PRICE`: preço médio dos imóveis naquela região

As variáveis preditoras (independentes) incluem:

- `MedInc`: Renda média da região  
- `HouseAge`: Idade média das casas  
- `AveRooms`: Média de cômodos por residência  
- `AveBedrms`: Média de quartos por residência  
- `Population`: População da região  
- `AveOccup`: Média de ocupação por residência  
- `Latitude`: Latitude da região  
- `Longitude`: Longitude da região  

---

## 🔧 Tecnologias Utilizadas

- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- scikit-learn  

---

## 📈 Resultados e Conclusões

Após treinar o modelo de regressão linear múltipla com todas as variáveis preditoras, os seguintes resultados foram obtidos:

- ✅ **Coeficientes:**
  ```text
  [ 4.48674910e-01   9.72425752e-03  -1.23323343e-01   7.83144907e-01
   -2.02962058e-06  -3.52631849e-03  -4.19792487e-01  -4.33708065e-01 ]
  ```

- ✅ **Intercepto:** `-37.02`

- ✅ **Coeficiente de determinação (R²):** `0.605`

O valor de R² indica que aproximadamente **60,5% da variabilidade do preço dos imóveis pode ser explicada pelas variáveis independentes** utilizadas no modelo. Isso mostra um ajuste razoável, mas sugere que outras variáveis também podem impactar o preço.

---

## 📊 Visualização dos Resultados

O gráfico abaixo mostra a relação entre os **preços reais** e os **preços previstos** pelo modelo:

```python
plt.scatter(y, y_pred)
plt.xlabel('Preço Real')
plt.ylabel('Preço Previsto')
plt.title('Preço Real vs Preço Previsto')
plt.plot([y.min(), y.max()], [y.min(), y.max()], 'k--', lw=2)
plt.show()
```

Se os pontos se aproximam da linha tracejada, isso indica boas previsões.
