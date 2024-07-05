# Aplicação de redes complexas para analisar como a cooperação é influenciada pela topologia da rede

No contexto de redes complexas, 'Cooperação'  é um campo de estudo que explora como agentes individuais (como pessoas, organizações, ou entidades biológicas) interagem e colaboram em sistemas interconectados e dinâmicos. 

Além disso, a topologia de uma rede complexa refere-se à estrutura e organização das conexões (arestas) entre os elementos (nós) da rede. É essencialmente o "mapa" de como os nós estão conectados uns aos outros. A topologia de uma rede complexa pode influenciar significativamente o comportamento e as propriedades dinâmicas da rede.

O projeto neste repositório busca entender como topologias diferentes (Erdős-Rényi, Watts-Strogatz e Barabási-Albert) podem estimular a cooperação de seus agentes envolvidos.

Para tanto, foram realizadas simulações utilizando um modelo baseado no dilema do prisioneiro iterado, um jogo amplamente utilizado para estudar a cooperação em sistemas dinâmicos. O dilema do prisioneiro iterado permite analisar como a cooperação pode emergir e se sustentar em um ambiente onde os agentes têm a opção de cooperar ou trair (defectar) em cada interação.

## Metodologia
### Geração das Redes:

- Erdős-Rényi: Redes geradas aleatoriamente onde cada par de nós tem a mesma probabilidade de estar conectado.
- Watts-Strogatz: Redes de mundo pequeno que introduzem aleatoriedade em uma rede regular, permitindo a presença de curtos caminhos globais e alta aglomeração local.
- Barabási-Albert: Redes livres de escala onde alguns nós (hubs) têm muitas conexões, enquanto a maioria tem poucas, seguindo uma distribuição de lei de potência.

### Implementação do Modelo de Cooperação:

- Cada nó da rede representa um agente que pode escolher entre cooperar ou trair.
- As interações entre agentes são determinadas pelas conexões (arestas) da rede.
- A tentação para traição é um parâmetro ajustável que influencia a decisão dos agentes de cooperar ou não.

### Simulações:

- Realização de múltiplas iterações para cada tipo de rede e configuração de parâmetros.
- Monitoramento da fração de agentes cooperadores ao longo do tempo.
- Variação da tentação para defecção para analisar seu impacto na cooperação.

## Resultados
### Redes Erdős-Rényi:

A cooperação tende a diminuir rapidamente com o aumento da tentação para defecção. Essas redes mostram uma menor robustez à cooperação comparadas às outras topologias.


### Redes Watts-Strogatz:

Apresentam uma maior robustez para cooperação, mantendo níveis relativamente altos de cooperação mesmo com aumentos na tentação para defecção. A estrutura de mundo pequeno facilita a manutenção de clusters cooperativos.

### Redes Barabási-Albert:

Redes com crescimento linear e sublinear mostram uma alta robustez à cooperação, mantendo níveis elevados de agentes cooperadores mesmo sob alta tentação para defecção.
Redes com crescimento superlinear, por outro lado, mostram uma robustez significativamente menor à cooperação.

# Conclusões
Este projeto demonstrou que a topologia da rede tem um impacto significativo na capacidade de uma rede manter níveis elevados de cooperação entre seus agentes. Redes Barabási-Albert lineares e sublineares são as mais eficientes em sustentar a cooperação, enquanto redes Erdős-Rényi são as menos eficientes. Redes Watts-Strogatz ocupam uma posição intermediária, combinando características de ambos os tipos de redes.

Os resultados sugerem que, ao projetar sistemas e redes para maximizar a cooperação (como em redes sociais, sistemas colaborativos e ecossistemas biológicos), a escolha da topologia é crucial. Redes com hubs bem conectados (como as Barabási-Albert) podem fornecer uma estrutura mais robusta para a cooperação, especialmente quando a tentação para defecção é alta.

# Aplicações Práticas Possíveis
- Redes Sociais: Entender como a estrutura da rede social pode promover a colaboração e reduzir comportamentos negativos.
Organizações: Projetar estruturas organizacionais que incentivem a cooperação entre os funcionários.
- Ecossistemas: Compreender como diferentes espécies interagem e colaboram em um ecossistema.

# Referências
- Playlist do prof. Francisco Rodrigues (também responsável pela matéria lecionada presencialmente no ICMC-USP): https://www.youtube.com/playlist?list=PLSc7xcwCGNh0HHNJlZBMBK6MzpdwNSzVT
- Cardillo, Alessio & Gómez-Gardeñes, Jesus & Vilone, Daniele & Sánchez, Angel. (2010). Coevolution of strategies and update rules in complex Prisoner's Dilemma networks. New Journal of Physics. 12. 103034. 10.1088/1367-2630/12/10/103034. 
- Poncela, J., Gómez-Gardeñes, J., Floría, L. M., & Moreno, Y. (2007). Robustness of cooperation in the evolutionary prisoner's dilemma on complex networks. New Journal of Physics, 9(6), 184. [doi: 10.1088/1367-2630/9/6/184]