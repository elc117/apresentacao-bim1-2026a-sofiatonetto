# apresentacao-bim1-2026a-sofiatonetto
apresentacao-bim1-2026a-sofiatonetto created by GitHub Classroom

Efeitos Colaterais
Quando a ação observada vai além do seu "efeito primário" -> ler e ou retornar um valor, alterando a saída programa sem ser pelo seu retorno.
Exemplos de efeitos colaterais: * O mais comum deles, atribuição de variáveis globais, pois são alteradas fora do escopo.
 * Uso de ponteiros: permitindo que a função altere o valor na memória.
 * Uso de operadores de Incremento ou Decremento: alteram o valor da variável.
> "Desvantagem Percebida": programas com efeitos colaterais faz com que o comportamento do código passa a depender da ordem de execução daquele programa, pois o valor de uma variável que está sendo usado pode ser modificado por uma função, por exemplo.
> 
Haskell e os efeitos colaterais:
Antes de entender isso precisei pesquisar mais sobre funções puras --> são livres de efeitos colaterais. Linguagens puramente funcionais permitem apenas o uso de 'funções puras'.
Propriedades úteis encontradas: * Se o resultado de uma função não é usado, a chamada dessa função é removida, não afetando outras expressões;
 * Processamento paralelo quando não há dependência de dados entre duas ou mais funções puras;
 * A função sempre vai retornar a mesma saída quando receber a mesma entrada;
Sobre a relação entre Haskell e os efeitos colaterais:
Todas suas funções são puras, pois tenta eliminar os efeitos colaterais. Porém existe algo chamado "Mônada" --> é uma estrutura algébrica que encapsula ações (como IO (entrada e saída, como ler arquivos e imprimir no terminal), Maybe (usado para computações que podem falhar ou retornos nulos) e List (quando uma função pode retornar múltiplos resultados) ao mesmo tempo que lida com os efeitos colaterais disso de forma pura.
Dados Imutáveis ou Imutabilidade:
Fundamental para programação funcional, garante que, depois de criados, os valores não podem ser modificados mais. Quando precisa alterar o estado, não deve ser alterado seu valor nunca, mas criado um.
Suas vantagens:
 * Evita efeitos colaterais já que uma vez que seus dados são criados, seus valores não podem ser alterados;
 * Facilita entendimento e debug do código: pelo fato de não permitir mudança nos dados, é mais fácil de entender como os dados são utilizados e onde, facilitando qualquer manutenção necessária.
Imutabilidade: Haskell não permite modificar variáveis diretamente; novos valores são criados em vez de alterar os antigos.
Referências:
 * Side Effect (Wikipedia)
 * Paradigmas de Programação - Efeitos Colaterais
 * Paradigmas de Programação - Funções Puras

