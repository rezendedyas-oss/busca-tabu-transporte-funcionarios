# Busca Tabu aplicada ao transporte de funcionários com janela de tempo

Este notebook apresenta a aplicação da heurística **Busca Tabu** ao problema de roteamento
de ônibus para transporte de funcionários, considerando restrições de horário de saída
e chegada.

---

## 1. Descrição do Problema

A empresa analisada disponibiliza transporte coletivo para seus funcionários, operando com
as seguintes características:

- Número de ônibus: 2  
- Ponto inicial: garagem da empresa  
- Horário de saída da garagem: 06:00  
- Horário máximo de chegada à empresa: 06:45  
- Número de pontos de embarque: 10
- Velocidade de média 80 km/h 

---

## 2. Metodologia – Busca Tabu

A **Busca Tabu** é uma meta-heurística baseada em busca local que explora iterativamente
o espaço de soluções, evitando ciclos por meio do uso de uma **lista tabu**.

Os principais elementos da Busca Tabu utilizados neste trabalho são:
- uma solução inicial viável
- uma estrutura de vizinhança
- uma lista tabu para evitar a repetição de movimentos
- a atualização contínua da melhor solução encontrada

As modificações aplicadas às soluções são do tipo **3-ops**, permitindo inversões,
trocas e realocações de clientes entre rotas.

---

## 3. Estrutura do Código

O código utilizado neste trabalho foi fornecido pelo professor da disciplina.
Foram realizadas adaptações apenas para fins de interpretação e apresentação dos resultados.

O algoritmo é composto pelas seguintes etapas:
- geração da vizinhança
- filtragem de movimentos proibidos (tabu)
- seleção do melhor vizinho
- execução iterativa da Busca Tabu

---

## 4. Implementação do Código

Google Colab 


## 5. Análise dos Resultados

Os resultados obtidos mostram que a Busca Tabu foi capaz de reduzir significativamente
o custo da solução inicial. As rotas finais apresentam melhor distribuição entre os
ônibus e menor distância total percorrida.

O gráfico gerado indica a convergência do algoritmo ao longo das iterações,
confirmando a eficiência da heurística aplicada ao problema proposto.

---

## 6. Conclusão

A heurística Busca Tabu mostrou-se adequada para o problema de roteamento de transporte
de funcionários com janela de tempo. O método é flexível, eficiente e pode ser aplicado
a problemas reais de maior porte, mantendo boas soluções em tempo computacional reduzido.
