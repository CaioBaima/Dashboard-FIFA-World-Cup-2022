# Dashboard-FIFA-World-Cup-2022
Elaborei um dashboard para que possamos acompanhar a copa do mundo com estatísticas em tempo real.


# COMO ATUALIZAR

Uma parte das consultas desse relatório vem de API. Esta API gera um token que deve ser inserido em "editor avançado".
Para gerar o token acesse o seguinte repositório https://github.com/raminmr/free-api-worldcup2022 onde o README explica como tudo deve ser feito.

Após gerar o token, basta acessar o relatório deste repositório, abrir o Power Query em "Transformar Dados", clicar em "editor avançado".

Nas linhas onde há:
```
Authorization = "Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJfaWQiOiI2MzcxOGQzZWZkOWFhYzIyNjdmNTRlOTQiLCJpYXQiOjE2NjkyNDIzMjcsImV4cCI6MTY2OTMyODcyN30.K3-ZA9IAa34IHer2bYDSJ7Nd0J6k5lP2jPpZVDSQG0Q",
```

mantenha a parte 
```
Authorization = "Bearer ", 
```
e insira após Bearer o seu token. Mantenha o formato do exemplo acima.

Esta alteração deve ser feita nos relatórios:
- Teams_API
- Matches_API
- Standings_API
