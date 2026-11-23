# Impacto do Ruído na Não-Localidade em Computadores Quânticos

**Autor:** Luan Almeida Meira  
**Orientador:** Pedro Silva Correia  
**Instituição:** Universidade Estadual de Santa Cruz (UESC), Brasil  
**Departamento:** DCEX – NEMeS  

---

## 🧭 Sobre o Projeto

Este projeto investiga o **impacto do ruído na não-localidade quântica** em computadores quânticos, utilizando a desigualdade de Bell na forma CHSH, tomografia de estados quânticos e simulações numéricas.

O estudo busca analisar como diferentes processos ruidosos afetam as correlações quânticas entre qubits logicamente distantes. Para isso, o distanciamento lógico entre Alice e Bob é implementado por meio de sucessivas portas **SWAP**, permitindo investigar como o ruído acumulado durante as operações quânticas influencia o emaranhamento e a violação da desigualdade de Bell.

São analisados diferentes modelos de ruído, individualmente e em combinação, buscando compreender seus efeitos sobre a preservação das correlações quânticas e da não-localidade.

---

## ⚛️ Fundamentação Teórica

### Desigualdade de Bell e cenário CHSH

As desigualdades de Bell estabelecem limites para as correlações previstas por teorias de variáveis ocultas locais. A desigualdade CHSH permite investigar a incompatibilidade entre as previsões da mecânica quântica e as teorias de realismo local, por meio de medidas realizadas em dois subsistemas.

O parâmetro CHSH é definido por:

\[
S=E(A_0,B_0)+E(A_0,B_1)+E(A_1,B_0)-E(A_1,B_1).
\]

Para teorias de variáveis ocultas locais, o limite é:

\[
|S|\leq 2.
\]

A violação desse limite indica correlações incompatíveis com modelos de variáveis ocultas locais.

### Emaranhamento quântico e distanciamento lógico

O trabalho utiliza um estado emaranhado de dois qubits como ponto de partida para o cenário de Bell. O distanciamento lógico entre os subsistemas é implementado por meio de sucessivas portas SWAP, permitindo investigar os efeitos da acumulação de ruído sobre as correlações quânticas.

Essa abordagem possibilita avaliar como as operações realizadas ao longo do circuito influenciam a preservação do emaranhamento e da violação da desigualdade CHSH.

### Tomografia de estados quânticos

A tomografia de estados quânticos permite reconstruir a matriz densidade do sistema de dois qubits (\(\rho_{AB}\)) a partir das estatísticas de medidas em diferentes bases.

A reconstrução do estado permite calcular diferentes métricas, possibilitando a caracterização do estado quântico após a aplicação das operações e dos processos ruidosos.

### Modelos de ruído

São investigados os seguintes processos ruidosos:

- **Ruído despolarizante:** provoca a degradação do estado quântico por meio da mistura com um estado maximamente misto.
- **Amplitude damping:** representa um processo de dissipação associado à perda de energia do sistema quântico.
- **Ruído combinado:** considera a atuação simultânea dos processos de ruído despolarizante e amplitude damping.

Esses modelos permitem investigar como diferentes mecanismos de ruído afetam as correlações quânticas e a violação da desigualdade de Bell.

---

## 🔬 Metodologia

O cenário de Bell ruidoso é implementado por meio do aumento do distanciamento lógico entre Alice e Bob, utilizando sucessivas portas SWAP.

A partir do circuito quântico, são obtidos dados de medidas que permitem realizar a tomografia do sistema de dois qubits e reconstruir sua matriz densidade. Os estados reconstruídos são utilizados para calcular o parâmetro CHSH e outras métricas de caracterização quântica.

A investigação compara os resultados obtidos para diferentes modelos de ruído, avaliando a degradação das correlações quânticas à medida que o distanciamento lógico aumenta.

### Métricas de análise

- **Parâmetro CHSH (\(S\)):** avalia as correlações quânticas e a violação da desigualdade de Bell.
- **Fidelidade:** quantifica a semelhança entre o estado ruidoso e o estado de referência.
- **Distância de traço:** quantifica a distinguibilidade entre estados quânticos.
- **Concorrência (Concurrence):** quantifica o emaranhamento quântico.
- **Negatividade (Negativity):** fornece uma medida adicional do emaranhamento.

---

## 📊 Objetivos

- Investigar o impacto do ruído na não-localidade quântica.
- Analisar como o aumento do distanciamento lógico afeta as correlações quânticas.
- Comparar os efeitos dos ruídos despolarizante e amplitude damping.
- Investigar os efeitos combinados de diferentes processos ruidosos.
- Avaliar a relação entre ruído, emaranhamento, fidelidade e violação da desigualdade CHSH.

---

## 💻 Ferramentas Utilizadas

- **Qiskit:** construção, execução e simulação de circuitos quânticos.
- **Python:** análise numérica, processamento de dados e visualização de resultados.
- **Tomografia de Estados Quânticos:** reconstrução de matrizes densidade.
- **Modelos de Ruído:** implementação e análise de processos ruidosos em sistemas quânticos.

---

## 📚 Referências Principais

- **Nielsen & Chuang (2010):** *Quantum Computation and Quantum Information*.
- **Bell (1964):** *On the Einstein Podolsky Rosen paradox*.
- **Clauser et al. (1969):** *Proposed Experiment to Test Local Hidden-Variable Theories*.
- **Horodecki et al. (1995, 1996):** estudos sobre violação de desigualdades de Bell e estados quânticos.
- **Brunner et al. (2014):** *Bell Nonlocality*.
- **Breuer & Petruccione (2002):** *The Theory of Open Quantum Systems*.
- **Vacchini (2024):** *Open Quantum Systems: Foundations and Theory*.
- **Wang et al. (2021):** *Bell inequalities for entangled qubits: quantitative tests of quantum character and nonlocality on quantum computers*.
- **Gårding et al. (2021):** *Bell Diagonal and Werner State Generation: Entanglement, Non-Locality, Steering and Discord on the IBM Quantum Computer*.
- **Yang et al. (2022):** *Testing Scalable Bell Inequalities for Quantum Graph States on IBM Quantum Devices*.
- **Storz et al. (2023):** *Loophole-free Bell inequality violation with superconducting circuits*.
- **Rico et al. (2024):** *Channel nonlocality under decoherence*.
- **Bönsel et al. (2025):** *Generating multipartite nonlocality to benchmark quantum computers*.
- **Cieśliński et al. (2025):** *How likely are you to observe non-locality with imperfect detection efficiency and random measurement settings?*.



