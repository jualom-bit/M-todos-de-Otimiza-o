Implementação em Python de dois métodos de otimização irrestrita
utilizando problemas padrão da biblioteca PyCUTEst: 

• Método Gradiente Descendente com busca de Armijo (GDA) [1]
• Método Espectral com variante não monótona (GBB) [2]

O código executa ambos os algoritmos no mesmo problema CUTEst, mede tempo,
iterações, norma do gradiente, avaliações de f e g, buscas lineares e 
buscas espectrais. Também produz um resumo comparativo automático entre os 
dois métodos, facilitando análise de desempenho e reproducibilidade.

Além disso, em um primeiro momento foram utilizados os parâmetros sugeridos em [1], e em um 
segundo momento empregou-se uma grade de variação (grid) para avaliar múltiplos 
modelos, permitindo observar melhorias e comparar o desempenho sob diferentes 
configurações.

Problemas CUTEst atualmente avaliados no projeto:
ARGLINA, ARGLINB, BA-L1SPLS, BIGGS6, BROWNAL, COATING,
FLETCHCR, GAUSS2LS, GENROSE, HAHN1LS, HEART6LS, HILBERTB,
HYDCAR6LS, LANCZOS1LS, LANCZOS2LS, LRIJCNN1, LUKSAN12LS,
LUKSAN16LS, OSBORNEA, PALMER1C, PALMER3C, PENALTY2, PENALTY3,
QING, ROSENBR, STRTCHDV, TESTQUAD, THURBERLS, TRIGON1, TOINTGOR.

------------------------------------------------------------
BIBLIOGRAFIA
------------------------------------------------------------

[1] J. Nocedal and S. J. Wright, *Numerical Optimization*, 2nd ed. Springer, 2006.

[2] M. Raydan, “The Barzilai and Borwein Gradient Method for the Large Scale 
Unconstrained Minimization Problem,” *SIAM J. Optim.*, vol. 7, no. 1, pp. 26–33, 1997.
