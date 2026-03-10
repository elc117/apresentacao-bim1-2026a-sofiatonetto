# apresentacao-bim1-2026a-sofiatonetto
apresentacao-bim1-2026a-sofiatonetto created by GitHub Classroom

Efeitos Colaterais 
  Qaundo a ação observada vai além do seu "efeito primário" -> ler e ou retornr um valor, alterando a saída programa sem ser pelo seu retorno. 
  Exemplos de efeitos colaterais: 
    * O mais comum deles, atribuição de variáveis globais, pois são alteradas fora do escopo.
    * Uso de ponteiros: permitindo que a função altere o valor na memória.
    * Uso de operadores de Incremento ou Decremento: alteram o valor da variável 

    "Desvantagem Percebida": programas com efeitos colaterais faz com que o comportamento do código passa a depender da ordem de execução daquele programa, pois o valor de uma variável que á sendo usado pode ser modificado por uma função,  por exemplo.
Haskell e os efeitos colaterais:
Antes de entender isso precisei pesquisar mais sobre funções puras --> são livres de efeitos colaterais. Lingiagens puramente funcionais permitem apenas o uso de 'f 'funções puras'.
          :-> propriedades úteis encontradas: 
                * se o resultado de uma função não é usado, a chamada dessa função é removida, não afetando outras expressões;
                * processamento paralelo quando não há dependência de dados entre duas ou mais funções puras;
                * A função sempre vai retornar a mesma saída quando receber a mesma entrada; 
Sobre a relação entre Haskell e os efeitos colaterais: é uma linguagem puramente funcional, ou seja, 
Haskell tenta eliminar os efeitos colaterais, então todas as funções são puras, a não ser que utilizemos E/S de dados
    
 Referências: 
 * https://en-wikipedia-org.translate.goog/wiki/Side_effect_(computer_science)?_x_tr_sl=en&_x_tr_tl=pt&_x_tr_hl=pt&_x_tr_pto=sge#:~:text=Realiza%C3%A7%C3%A3o%20de%20E/S.,MIT%20Press%20.(efeitos colaterais)
 * https://leandromoh.gitbooks.io/tcc-paradigmas-de-programacao/content/5_paradigma_funcional/52_efeitos_colaterais.html (efeitos colaterais)
