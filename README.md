# AOSC 2023 - Problemas para resolução na linguagem Delégua

Nesta mentoria, o mentorado é convidado a implementar três jogos típicos de cassinos, na seguinte ordem:

- Roleta
- Craps (Dados)
- Blackjack (Vinte e um)

[Veja como experimentar ou instalar Delégua aqui](https://github.com/DesignLiquido/delegua). [O manual de referência da linguagem está aqui](https://github.com/DesignLiquido/delegua/wiki).

## Roleta

O objetivo dos jogadores quanto ao jogo de Roleta que é jogada em cassino vai muito além de ganhar dinheiro e fazer uma aposta. Seu objetivo ao jogar é fazer suas apostas e escolher o número vencedor que aparecerá na “roda pequena” (“Roulette” em francês). 
Os jogadores podem apostar em combinações de números, escolher a cor, ou até mesmo se o número será par ou ímpar.

### Como jogar

No jogo de roleta o jogador deve depositar sua ficha, que representa o valor da jogada, sobre o tipo de aposta que deseja realizar. O croupier gira a roleta e lança a bola. O jogador ganha se a bola parar na casa correspondente a de sua aposta. 
Há diferenças entra a roleta americana e a roleta européia. A roleta americana dá um pouco mais de vantagem para a banca em comparação com a roleta europeia. O motivo é a existência da casa 00.

Roleta tem uma grande variedade de apostas e prêmios. As apostas individuais, por exemplo, acontecem na parte de dentro da mesa, quando o jogador escolhe um determinado número (de uma determinada cor). Esse tipo de aposta é a que paga os maiores prêmios (35 a 1). 
Ao mesmo tempo, são as jogadas com menor probabilidade de acerto.

Outros tipos de aposta que acontecem na parte de dentro da mesa:

- Dupla: aposta em dois números ao mesmo tempo. Podem ser vizinhos verticalmente ou horizontalmente.
- Rua: aposta em 3 números na orientação horizontal.
- Rua Dupla: aposta em 6 números vizinhos horizontalmente.
- Quadrado ou canto: aposta em 4 números que formam um quadrado.
- Trio: aposta nos três primeiros números da mesa: 0/00/1 (na roleta americana) / 0/1/2 (na roleta europeia).

As apostas do lado de fora da mesa são as menos ousadas, mas também podem dar grandes lucros para o jogador sem que ele corra grandes riscos. A probabilidade de vitória em algumas dessas jogadas é de 49%. No entanto, os prêmios são menores se comparados aos das apostas da parte interna da mesa, pagando 2x1. Confira as apostas do lado externo da mesa:

- Vermelho ou Preto: todos os números da mesa possuem coloração preta ou vermelha (com exceção ao 0). O jogador aposta que o próximo número será da cor vermelha ou preta. A probabilidade de vitória é de 49%, e essa aposta paga 2x1.
- Par ou ímpar: o jogador prevê se o próximo número sorteado será par ou ímpar. Essa jogada pode ser realizada em conjunto com a vermelho/preto, para aumentar sua premiação.
- Aposta de dúzias: na roleta americana há 38 números, e na roleta europeia são 37. Esses números são divididos em 3 dúzias (excluindo os números nulos). O jogador pode apostar qual delas terá um número sorteado.
- Aposta de Coluna: a mesa do jogo de roleta é dividida em três colunas. A exemplo da aposta de dúzias, o jogador pode realizar sua jogada em alguma dessas colunas.
- 1-18 / 19-36: Aposta que prevê que o número sorteado fará parte de alguma das divisões da mesa.

## Craps (Dados)

Craps é um jogo realizado em uma mesa com marcações das apostas e dois dados. Dependendo do resultado dos dados, os jogadores ganham determinadas premiações. 

### Como jogar

Craps é organizado por rodadas. Independente do momento de cada rodada, todos os jogadores podem apostar da seguinte forma:

- Diretamente nos números 4, 5, 6, 8, 9 ou 10: se a rolagem tiver como resultado um desses números, e houver fichas no número, os jogadores que apostaram nesse número são premiados. Se a rolagem for um 7, a casa fica com as fichas;
- Contra os números 4, 5, 6, 8, 9 ou 10: se a rolagem atual tiver como resultado um desses números, e houver fichas contra o número, a casa fica com as fichas. Se a rolagem for um 7, a casa paga para cada ficha outra ficha do mesmo valor, devolvendo as fichas originais aos respectivos jogadores;
- Dados iguais ("hard ways"): para números pares (4, 6, 8 ou 10), cada jogador pode apostar em números com resultado específico de dados iguais (respectivamente, 2 e 2, 3 e 3, 4 e 4, 5 e 5). Se o resultado for um desses números e os valores dos dados forem iguais, cada jogador recebe sete vezes o valor apostado (para 6 e 8), ou nove vezes o valor apostado (para 4 ou 10). No entanto, se o resultado for um número par com valores entre os dados diferentes, ou se a rolagem for um 7, a casa fica com as fichas;
- Diretamente nos números 2 ou 12: se a rolagem tiver como resultado um desses números, e houver fichas no número, os jogadores que apostaram nesse número são premiados. Diferentemente das apostas anteriores, se a rolagem for qualquer outro número, a casa fica com as fichas. Por isso, aqui é uma das premiações mais altas: 30 fichas para cada ficha apostada;
- Diretamente nos números 3 ou 11: se a rolagem tiver como resultado um desses números, e houver fichas no número, os jogadores que apostaram nesse número são premiados. Assim como na aposta direta em 2 ou 12, se a rolagem for qualquer outro número, a casa fica com as fichas. A premiação aqui é de 15 fichas para cada ficha apostada;
- Diretamente no número 7: se a rolagem tiver como resultado qualquer sete, e houver fichas no número, os jogadores que apostaram no 7 são premiados. Assim como nas apostas diretas em 2, 3, 11 ou 12, se a rolagem for qualquer outro número, a casa fica com as fichas. A premiação aqui é de 5 fichas para cada ficha apostada;
- "Any Craps", ou simplesmente "Craps": se a rolagem tiver como resultado 2, 3 ou 12, e houver fichas nessa posição, os jogadores que apostaram aqui são premiados. Assim como nas apostas diretas em 2, 3, 7, 11 ou 12, se a rolagem for qualquer outro número, a casa fica com as fichas. A premiação aqui é de 8 fichas para cada ficha apostada;
- "Field": se a rolagem tiver como resultado 2, 3, 4, 9, 10, 11 ou 12, e houver fichas nessa posição, os jogadores que apostaram aqui são premiados. Assim como nas apostas diretas em 2, 3, 7, 11 ou 12, ou "Any Craps", se a rolagem for qualquer outro número, a casa fica com as fichas. A premiação aqui é de uma ficha para cada ficha apostada;
- "High": se a rolagem tiver como resultado qualquer número de 8 a 12, e houver fichas nessa posição, os jogadores que apostaram aqui são premiados. Assim como nas apostas diretas em 2, 3, 7, 11 ou 12, "Any Craps" ou "Field", se a rolagem for qualquer outro número, a casa fica com as fichas. A premiação aqui é de uma ficha para cada ficha apostada;
- "Low": se a rolagem tiver como resultado qualquer número de 2 a 6, e houver fichas nessa posição, os jogadores que apostaram aqui são premiados. Assim como nas apostas diretas em 2, 3, 7, 11 ou 12, "Any Craps", "Field" ou "High", se a rolagem for qualquer outro número, a casa fica com as fichas. A premiação aqui é de uma ficha para cada ficha apostada.

Em algumas meses, as posições 2, 3, 7, 11, 12, "Any Craps", "Field", "High" ou "Low" são pintadas com letras douradas. Posições em letras douradas são chamadas de "Single Rolls" (rolagens únicas), porque cada rolagem define se o jogador ganha e perde. As demais posições, normalmente pintadas em branco, são definidas ou com resultado de uma rolagem, ou com o fim de uma rodada (quando o lançador rola um 7).

#### Nova rodada e momento de linha de passe

Para cada nova rodada, um dos jogadores é eleito o lançador que, além de lançar os dados, é obrigado a fazer pelo menos uma aposta inicial no momento chamado "linha de passe" ("come out roll"). Os outros jogadores podem apostar como quiserem.

No momento da linha de passe, dois espaços na mesa podem receber fichas e dois outros não podem: os que podem são chamados de "pass" ("passar") e "don't pass" ("não passar"), e os que não podem são o "come" ("virar resultado") e "don't come" ("não virar resultado"). Neste primeiro momento, cada espaço premia da seguinte forma:

- Quem apostou em "pass" vence quando o resultado do lançamento é 7 ou 11. Esse resultado é chamado de "Natural";
- Quem apostou em "don't pass" vence quando o resultado do lançamento é 2 ou 3. Quando o resultado é 12, algumas versões pagam uma ficha para cada ficha apostada, ou as fichas são simplesmente devolvidas aos jogadores. Este resultado é chamado de "Crap Out";
- Para quaisquer outros resultados (4, 5, 6, 8, 9 ou 10), as fichas permanecem nas respectivas posições até o final da rodada. O número sorteado passa a ser o "ponto" ("point") da rodada.

Os resultados "Natural" e "Crap Out" permitem aos jogadores apostar novamente em "pass" e "don't pass" para os lançamentos seguintes. Para os demais resultados, as posições "pass" e "don't pass" não podem mais receber fichas até o final da rodada, e as posições "come" e "don't come" passam a aceitar fichas, também até o final da rodada.

#### Momento de ponto definido

