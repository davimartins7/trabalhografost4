# Traveling Salesman Problem (TSP)

## Heurísticas de Inserção: Nearest vs Smallest

---

## 📌 Sobre o Projeto

Este trabalho implementa duas heurísticas clássicas para o problema do **Caixeiro Viajante (TSP)**:

- **Nearest Insertion**
- **Smallest (Cheapest) Insertion**

O objetivo **não é encontrar a solução ótima**, mas comparar o comportamento das heurísticas na construção de circuitos (*tours*).

---

## 🎯 Objetivo

- Modelar cidades como pontos 2D  
- Calcular distância euclidiana  
- Construir circuitos incrementalmente  
- Comparar heurísticas  
- Visualizar os resultados  

---

## 🧠 Heurísticas Implementadas

### **Nearest Insertion**

- Escolhe a cidade mais próxima do circuito atual  
- Insere na melhor posição possível  

**Foco:** proximidade local  

---

### **Smallest (Cheapest) Insertion**

- Testa todas as possíveis inserções  
- Escolhe a que gera menor aumento no percurso  

**Foco:** custo global  

---

## ⚖️ Diferença Principal

- **Nearest:** escolhe a cidade primeiro, depois a posição  
- **Smallest:** escolhe diretamente a melhor inserção  

---

## 🐍 Tecnologias Utilizadas

- Python 3  
- Matplotlib (visualização)  
- Estrutura baseada em **algs4**  

---

## 📂 Estrutura do Código

O projeto foi desenvolvido em **blocos (Google Colab)**:

### **Bloco 1**
- Download do repositório base (`algs4`)
- Download do arquivo `usa13509.txt`
- Importações (`math`, `matplotlib`, `time`)

---

### **Bloco 2**
- Implementação do `StdDraw` (simulação com matplotlib)
- Classe `Point`
  - Representação das cidades
  - Cálculo de distância

---

### **Bloco 3**
- Classe `Tour`
  - Lista encadeada circular
  - Métodos principais:
    - `insertNearest(Point p)`
    - `insertSmallest(Point p)`
    - `length()`
    - `draw()`

---

### **Bloco 4**
Execução das heurísticas:

- `run_nearest()` → executa Nearest  
- `run_smallest()` → executa Smallest  
- `run_compare()` → comparação visual  

---

## ▶️ Como Executar

### **Google Colab (Recomendado)**

1. Execute o **Bloco 1** para baixar dependências  
2. Execute os blocos na ordem (1 → 4)  
3. O programa irá gerar:

- Visualização do Nearest  
- Visualização do Smallest  
- Comparação entre os dois  

## 📊 Saída

O programa exibe:

- Número de pontos  
- Comprimento do tour (Nearest)  
- Comprimento do tour (Smallest)  
- Visualização gráfica dos circuitos  

---

## 🧪 Arquivo Utilizado

- `usa13509.txt` → instância principal (13.509 cidades)

---

## 🎥 Vídeo Explicativo

**Link do vídeo:**  
👉 https://youtu.be/szpLUkXO_DA

---

## 👨‍💻 Autores

- Davi Martins 
- Isaac Coelho
- Paulo Afonso 

---

## 📌 Observação Final

O projeto segue o padrão da disciplina (**algs4**) e foca na implementação correta das heurísticas e na comparação dos resultados obtidos.
