## - Curso Alura -
# Python: Avançando na linguagem

Nesse curso oferecido pela Alura, foi implantado um jogo da forca, utilizando as estruturas de dados, listas e outras sequências. 

1. No jogo da forca o usuário deve adivinhar uma palavra secreta. No arquivo forca.py, já há a função jogar definida, onde consta o código do  jogo. 
2. While: Utilizamos a condição do while para controlar a execução do jogo da Forca, ou seja, enquanto o jogador não acertar a palavra secreta e não enforcar o bonequinho na forca, o loop continuará a ser executado.

    A condição (not enforcou and not acertou) no while é avaliada a cada iteração do loop. Se a condição for verdadeira, o loop continuará executando. Se a condição for falsa, o loop será interrompido e a mensagem "Fim do jogo" será exibida.

    Dentro do loop, o jogador é solicitado a informar uma letra e a lista de letras acertadas é atualizada com a letra correta, caso o jogador tenha acertado. Se o jogador acertar todas as letras da palavra secreta, a variável acertou será definida como True, encerrando o loop e exibindo a mensagem de "Fim do jogo". Se o jogador errar muitas vezes e a variável enforcou for definida como True, também ocorrerá a mesma coisa, encerrando o loop e exibindo a mensagem de "Fim do jogo".

    > Break = quando executada, encerra o loop naquele ponto. 

3. Funções de String utilizadas:
   >  Upper: utilizada para converter as letras informadas pelo jogador e as letras da palavra secreta em letras maiúsculas, permitindo que a comparação de letras seja feita independentemente se elas foram informadas em maiúsculas ou minúsculas. Isso é importante para evitar erros no jogo, já que as letras maiúsculas e minúsculas são tratadas de forma diferente em Python. Se o jogador informar a letra em minúscula e a letra correta da palavra secreta estiver em maiúscula, a comparação falhará e a letra não será considerada como correta, causando um erro no jogo.

   > Strip: utilizada para remover espaços em branco (ou outros caracteres especificados) no início e fim da string informada pelo jogador no momento em que ele informa uma letra como chute. Essa função é importante para garantir que a entrada do jogador seja válida e para evitar erros no jogo. Se o jogador digitar um espaço ou outro caractere indesejado antes ou depois da letra que ele deseja informar, a função strip() removerá esses caracteres e a comparação da letra informada com as letras da palavra secreta será feita de forma correta.

4. Lista:  uma estrutura de dados em Python que permite armazenar um conjunto de valores em uma única variável. Cada valor na lista é separado por vírgulas e pode ser acessado através de um índice numérico que começa a partir de zero. As listas são dinâmicas, ou seja, podem ser modificadas adicionando ou removendo elementos. Por exemplo, para adicionar um novo elemento à lista, podemos usar o método append. E para remover um elemento da lista, podemos usar o método remove.

    O código utiliza listas em diversas partes do programa. Algumas funções que utilizam listas no código são:

* inicializa_letras_acertadas(palavra): Essa função recebe uma string palavra e cria uma lista de tamanho igual ao número de caracteres da palavra, preenchendo-a com o caractere "_". Essa lista representa as letras acertadas pelo jogador até o momento.

* marca_chute_correto(chute, letras_acertadas, palavra_secreta): Essa função recebe um caractere chute, a lista letras_acertadas e a string palavra_secreta. Ela itera pelos caracteres da string palavra_secreta, verificando se o caractere chute está presente em algum deles. Se estiver, a função atualiza a lista letras_acertadas, atribuindo o caractere chute na posição correspondente na lista.

* carrega_palavra_secreta(): Essa função lê um arquivo chamado "palavras.txt" e armazena cada linha desse arquivo em uma lista chamada palavras. Em seguida, a função sorteia um índice aleatório da lista palavras e retorna a palavra secreta correspondente, em forma de string.

5. Funções: O código foi dividido em funções para facilitar a organização do código e torná-lo mais fácil de ler, entender e manter. Além disso, dividir o código em funções torna-o mais modular, o que significa que cada função pode ser testada e depurada separadamente. 