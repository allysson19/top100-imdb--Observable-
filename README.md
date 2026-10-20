# Top 100 IMDB Movies: rede de filmes, diretores e atores

Visualização em rede (D3, force-directed) com os 100 filmes mais bem avaliados do IMDB, seus diretores e os dois atores principais de cada filme.

**Notebook no Observable:** https://observablehq.com/d/4d2d6b9fea2e6623

## Dados

- Arquivo: `imdb_data_100_2026_2.json`
- 323 nós (100 filmes, 64 diretores, 159 atores) e 300 ligações
- Cada filme se liga a 1 diretor e 2 atores (`actor1` e `actor2`)

## Codificação visual

- **Cor:** tipo de nó (vermelho = filme, azul = diretor, laranja = ator)
- **Tamanho:** nota do IMDB para filmes; número de filmes no dataset para diretores e atores
- **Tooltip:** nome, tipo e detalhes (ano, nota, rank, diretor e elenco para filmes; número de filmes para pessoas)
- **Interação:** ao passar o mouse, os nós ligados ficam em destaque

## Respostas

**Que diretor dirigiu mais filmes no dataset? Quantos e quais filmes ele dirigiu?**

Christopher Nolan, com 7 filmes: Memento (2000), The Prestige (2006), The Dark Knight (2008), Inception (2010), The Dark Knight Rises (2012), Interstellar (2014) e The Odyssey (2026). Na visualização, ele é o maior nó azul e tem 7 ligações com nós vermelhos (filmes). O segundo colocado é Quentin Tarantino, com 4 filmes.

**Que ator participou de mais filmes no dataset? Quantos e de quais filmes ele participou?**

Tom Hanks, com 5 filmes: Forrest Gump (1994), Toy Story (1995), Saving Private Ryan (1998), The Green Mile (1999) e Toy Story 3 (2010). Na visualização, ele é o maior nó laranja e tem 5 ligações com filmes. O dataset traz apenas dois atores por filme, então a contagem vale para o elenco principal listado.
