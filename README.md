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

- CUSTO FINAL (com penalidade se houver): 10173.2

ROTAS FINAIS E TEMPOS:

Ônibus 1
Rota: [0, 4, 3, 1, 2, 5, 10]
Distância total: 81.60 km
Tempo total: 61.20 minutos
✖ Violou a janela de tempo

Ônibus 2
Rota: [0, 6, 7, 8, 9, 10]
Distância total: 91.60 km
Tempo total: 68.70 minutos
✖ Violou a janela de tempo

- Precisaria de mais tempo, desta forma saindo mais cedo
  

## 6. Considerações finais 

- Trabalhos futuro
- Desafios
  


