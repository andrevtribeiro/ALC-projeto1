O programa começa por ler o input dado (número de nodes, número de features e as samples).
Após a leitura do input, o programa chama a função enc que por sua vez chama as funções create_tree_constraints (esta função é responsável por criar as constraints para a codificação de árvores binárias) e a função create_decision_constraints (esta função é responsável pela criação das constraints associadas à computação de árvores de decisão tendo em conta as samples que recebe como input).
Depois de criadas todas as constraints, estas são passadas para formato CNF e é chamado o SAT solver (lingeling) para resolver o problema, caso o problema tenha solução é chamada a função print_output que imprime a solução do problema, caso este não tenha solução o output do programa é UNSAT.

André Ribeiro Nº86384
Paulo Dias    Nº86492
