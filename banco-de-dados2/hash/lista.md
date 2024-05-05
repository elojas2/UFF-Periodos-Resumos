### Exercício 1. 
Não discutimos como exclusões são executadas em tabelas hash dinâmicas
(lineares E extensíveis). Assumindo que a estratégia de busca é direta, qual método você
sugere para excluir uma entrada do hash? Quais as vantagens e desvantagens de reestruturar
a tabela depois da exclusão de certos blocos para mantê-la compacta?


Resposta: Como precisamos excluir de forma direta, basta localizar (buscar) na tabela hash usando uma função de sondagem (o que foi nos ensinado foi a sondagem linear, ela funciona da seguinte maneira, se ocorre uma colisão na posição de uma certa chave, essa função irá procurar pela próxima posição livre na tabela de forma linear).

Excluindo então na tabela e realocando os ponteiros para que mantenha a "ordem".

Reestruturar a tabela tem vantagens como melhoramento do desempenho da mesma, tanto no tempo de busca quanto de memória.

Já nas desvantagens, terá um custo maior para fazer a restruturação já que remover e reorganizar os dados demanda tempo e desempenho. Relacionado com o desempenho, teremos a complexidade de implementar a restruturação também. 



### Exercício 2. 
Utilize sua resposta do exercício anterior para discutir a operação de atualização de valor de uma chave.


### Exercício 3. 
Nas aulas, assumimos que os valores das chaves são únicos, o que não precisa
ser o caso para o uso de hash. No entanto, apenas algumas pequenas modificações são necessárias para buscar chaves com valores duplicados (ou mais). Descreva as mudanças necessárias para os algoritmos de inserção e busca para lidar com chaves não únicas, considerando hash (a) estático, (b) extensível e (c) linear.


### Exercício 4. 
Algumas funções hash não funcionam muito bem (quando comparadas a outras
mais adequadas). Suponha a função h(x) para x inteiro onde h(x) = x^2 mod B, onde B é o
número de buckets.
a) O que acontece com essa função se B = 10?
b) Quão boa é essa função se B = 16?
c) Existe valor de B para o qual essa função é útil?


### Exercício 5. 
Suponha que foi usado o método da “dobra” e a função de hash gere uma saída
de 4 bits, ou seja, h(x) -> [0,1]^4. Suponha também que os buckets suportam três chaves sem
overflow. Se iniciarmos o hash com dois buckets vazios (indexados por um array com uma
entrada 0 e outra 1, ou seja um array de 1 bit), mostre o passo-a-passo da inserção das
seguintes chaves:
a) 0000,0001,... ,1111 e o método é hash extensível.
b) 0000,0001,... ,1111 e o método é hash linear com taxa de ocupação de 150%.
c) 1111,1110,..., 0000 e o método é hash extensível.
d) 1111,1110,... , 0000 e o método é hash linear com taxa de ocupação de 120%.