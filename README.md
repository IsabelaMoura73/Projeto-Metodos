# 🫀 Potenciais das Células Cardíacas Humanas utilizando o Modelo de FitzHugh–Nagumo

Projeto desenvolvido para a disciplina **Métodos Numéricos**, com o objetivo de modelar, simular e analisar a dinâmica dos potenciais de ação de células cardíacas humanas utilizando o modelo de FitzHugh–Nagumo — uma versão simplificada do modelo de Hodgkin–Huxley, amplamente utilizado para descrever impulsos elétricos em células excitáveis.

## 👩‍🔬 Integrantes do Grupo

- Carolina Gabriela de Arruda Brito dos Santos
- Isabela Maria de Moura Nascimento
- Karina Lima de Oliveira
- Kauanny Karolinna D'Avalon Araujo e Barros
- 
## 🎓 Sobre o Projeto

O coração humano é um sistema auto-oscilante capaz de gerar e propagar impulsos elétricos que regulam o ritmo cardíaco. Esses impulsos resultam de variações no potencial de membrana de dois tipos principais de células:

- **Células marca-passo** – geram espontaneamente os impulsos elétricos que iniciam cada batimento cardíaco.  
- **Células miocárdicas** – propagam o sinal elétrico e promovem a contração do músculo cardíaco.

Este projeto visa reproduzir e analisar a dinâmica desses potenciais de ação por meio do **modelo de FitzHugh–Nagumo (FHN)**, que reduz o sistema original de quatro equações diferenciais (Hodgkin–Huxley) para apenas duas, mantendo as características essenciais de excitabilidade com menor custo computacional.

Além disso, simulamos a **interação elétrica entre células cardíacas** através de um parâmetro de acoplamento \( K \), representando a eficiência das **junções comunicantes (gap junctions)**.

## 🎯 Objetivos do Projeto

- Implementar numericamente o sistema de FitzHugh–Nagumo com o método de **Runge-Kutta de 4ª ordem**.  
- Simular e comparar diferentes tipos de estímulo externo \( I(t) \):  
  - Constante  
  - Onda quadrada (células miocárdicas)  
  - Onda cossenoidal (células marca-passo)  
- Analisar propriedades como ciclos-limite, pontos fixos e estabilidade linear.  
- Investigar o impacto do acoplamento elétrico \( K \) na sincronização entre células.  
- Reproduzir comportamentos fisiológicos (ritmo saudável) e patológicos (dessincronização).

## 📊 Resultados Obtidos

Foram simulados três cenários de acoplamento elétrico:

| Valor de K | Comportamento do Sistema | Interpretação Fisiológica |
|------------|---------------------------|----------------------------|
| **0.08**   | Dessincronizado           | Comunicação deficiente (patologia severa) |
| **2.0**    | Sincronização parcial     | Condução degradada (fibrose leve, envelhecimento) |
| **5.0**    | Sincronização quase perfeita | Tecido saudável com propagação eficiente |

Foram geradas visualizações de:
- Evolução temporal dos potenciais de ação  
- Diferença de potencial |x₁ - x₂| ao longo do tempo  
- Retratos de fase x₁ × x₂

Esses resultados evidenciam a transição entre estados fisiológicos e patológicos conforme a variação do acoplamento.

## 🛠️ Tecnologias Utilizadas

- **Python** – linguagem principal para simulação  
- **NumPy** – operações numéricas e manipulação de vetores  
- **Matplotlib** – geração de gráficos e visualização de resultados  
- **Google Colab / Jupyter Notebook** – ambiente de desenvolvimento e experimentação

## 📈 Conclusões

O modelo acoplado de **FitzHugh–Nagumo**, apesar de simplificado, mostrou-se altamente eficaz para representar qualitativamente os processos de geração, propagação e sincronização dos potenciais de ação em células cardíacas.  

A análise do parâmetro de acoplamento K permitiu identificar transições entre diferentes regimes de sincronização, correlacionando diretamente com estados fisiológicos (tecido saudável) e patológicos (arritmias e falhas de condução).

✅ **Principais Contribuições:**
- Simulação precisa de fenômenos cardíacos com baixo custo computacional.  
- Análise quantitativa da importância do acoplamento elétrico.  
- Base para estudos futuros envolvendo modelos mais complexos ou heterogeneidade celular.
