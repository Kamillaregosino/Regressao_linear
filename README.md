# 📊 Regressão Linear Simples – Prevendo Notas com Base em Horas de Estudo

Este projeto demonstra como aplicar uma **regressão linear simples** usando Python para prever a nota de um estudante com base em quantas horas ele estudou. O objetivo é mostrar a relação entre uma variável independente (horas de estudo) e uma variável dependente (nota obtida).

## 📁 Sobre o Dataset

O conjunto de dados contém apenas duas colunas:

- `Hours`: número de horas estudadas
- `Scores`: nota final obtida

Fonte: [GitHub - student_scores.csv](https://raw.githubusercontent.com/AdiPersonalWorks/Random/master/student_scores%20-%20student_scores.csv)

---

## 🔧 Tecnologias Utilizadas

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

---

## 📈 Resultados e Conclusões

Após treinar o modelo, os seguintes resultados foram obtidos:

- ✅ **Coeficiente angular (slope):** `9.68`
- ✅ **Intercepto (intercept):** `2.83`
- ✅ **Erro médio absoluto (MAE):** `3.92`
- ✅ **Coeficiente de determinação (R²):** `0.97`

Esses resultados indicam que há uma **forte correlação linear positiva** entre as horas estudadas e as notas dos alunos. Em média, **a cada hora adicional de estudo, a nota aumenta cerca de 9.68 pontos**.

### 🎯 Exemplo de Previsão

Se um aluno estudar **6 horas**, a nota prevista será: Nota = 9.68 * 6 + 2.83 = 60.91

