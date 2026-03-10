# apresentacao-bim1-2026a-sofiatonetto
apresentacao-bim1-2026a-sofiatonetto created by GitHub Classroom

Efeitos Colaterais 
  Quando a ação observada vai além do seu "efeito primário" -> ler e ou retornr um valor, alterando a saída programa sem ser pelo seu retorno. 
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
                
Sobre a relação entre Haskell e os efeitos colaterais: 
                      todas suas funções são puras, pois tenta eliminar os efeitos colaterais
                      Porém existe algo chamado "Mônada" --> é uma estrutura algébrica que encapsula ações (como IO (entrada e saída, como ler arquivos e imprimir no terminal) , Maybe (usado para computações que podem falhar ou retornos nulos) e List (quando uma função pode retornar múltiplos resultados) ao mesmo tempo que lida com os efeitos colaterais disso de forma pura. 

Dados Imutáveis ou Imutabilidade: fundamental para programação funcional, garante que, depois de criados, os valores não podem ser modificados mais. Quando precisa alterar o estado, não deve ser alterado seu valor nunca, mas criado um. 
Suas vantagens:
  *evita efeitos colaterais ja que uma vez que seus dados são criados, seus valores não podem ser alterados; 
  *facilita entendimento e debug do código: pelo fato de não permitir mudança nos dados, é mais fácil de entender como os dados sao utlizados e onde, facilitando qualquer manutenção necessária.

Imutabilidade: Haskell não permite modificar variáveis diretamente; novos valores são criados em vez de alterar os antigos.
    
 Referências: 
 * https://en-wikipedia-org.translate.goog/wiki/Side_effect_(computer_science)?_x_tr_sl=en&_x_tr_tl=pt&_x_tr_hl=pt&_x_tr_pto=sge#:~:text=Realiza%C3%A7%C3%A3o%20de%20E/S.,MIT%20Press%20.(efeitos colaterais)
 * https://leandromoh.gitbooks.io/tcc-paradigmas-de-programacao/content/5_paradigma_funcional/52_efeitos_colaterais.html (efeitos colaterais)
 * https://leandromoh.gitbooks.io/tcc-paradigmas-de-programacao/content/5_paradigma_funcional/53_funcoes_puras.html (funcoes puras)


Efeitos Colaterais (Side Effects)
Um efeito colateral ocorre quando a ação de uma função vai além do seu efeito primário (retornar um valor), alterando o estado do sistema ou a saída do programa de forma externa ao seu escopo imediato.
Exemplos Comuns:
 * Variáveis Globais: Alterações de valores fora do escopo local.
 * Ponteiros: Funções que modificam diretamente o valor alocado na memória.
 * Operadores de Incremento/Decremento: Alteração direta do valor da variável original.
> Desvantagem Percebida: Programas com efeitos colaterais tornam o comportamento do código dependente da ordem de execução. Isso dificulta a previsão do estado da variável em diferentes momentos do programa.
> 
Haskell e as Funções Puras
Para entender como Haskell lida com isso, é necessário compreender o conceito de Funções Puras, que são a base das linguagens puramente funcionais.
Propriedades das Funções Puras:
 * Determinismo: A função sempre retorna a mesma saída para a mesma entrada.
 * Transparência Referencial: Se o resultado não é usado, a chamada pode ser removida sem afetar o programa.
 * Paralelismo: Facilita o processamento paralelo, pois não há dependência de dados entre funções independentes.
O papel das Mônadas
Haskell elimina efeitos colaterais em funções comuns, mas utiliza Mônadas para gerenciar interações necessárias com o "mundo real" de forma controlada e pura.
 * IO: Entrada e saída (leitura de arquivos, terminal).
 * Maybe: Gerenciamento de falhas ou retornos nulos.
 * List: Lida com múltiplos resultados possíveis.
Imutabilidade
A imutabilidade é o pilar que garante que, uma vez criado, um valor nunca seja modificado. Se você precisa de um "novo estado", você cria um novo dado em vez de alterar o antigo.
Vantagens da Imutabilidade:
| Vantagem | Descrição |
|---|---|
| Previsibilidade | Evita efeitos colaterais inesperados. |
| Debug Facilitado | Como os dados não mudam, é mais fácil rastrear o fluxo da informação. |
| Segurança | Reduz erros comuns em sistemas complexos e concorrentes. |
Referências
 * Side Effect - Wikipedia (PT-BR)
 * Paradigmas de Programação: Efeitos Colaterais
 * Paradigmas de Programação: Funções Puras

