Neural Evolution Augmenting Topology
- Rede Neural

Inputs:
Posição do Pássaro Y
Distancia do Passaro pro cano de Cima
Distancia do Passaro pro cano de Baixo

Output:
Pula?

Funciona Por pesos
Posição do Pássaro Y - 0.5
Distancia do Passaro pro cano de Cima - 2
Distancia do Passaro pro cano de Baixo - 1.3

Soma um Bias no final

Aplica uma tangente hiperbolica para condensar todos os resultados entre 0 e 1
Acima de 0.5 Pula
Abaixo Não Pula

Inicialmente os numeros de pesos e Bias Sao definidos pela IA aleatoriamente

100 Pássaros a cada geração
