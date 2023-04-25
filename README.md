## - Curso Alura -
# Python: Avançando na linguagem

Nesse curso oferecido pela Alura, foi implantado um jogo da forca, utilizando as estruturas de dados, listas, tuplas e outras sequências. 

1. No jogo da forca o usuário deve adivinhar uma palavra secreta. No arquivo forca.py, já há a função jogar definida, onde consta o código do  jogo. 
2. While: Utilizamos a condição do while para controlar a execução do jogo da Forca, ou seja, enquanto o jogador não acertar a palavra secreta e não enforcar o bonequinho na forca, o loop continuará a ser executado.

    A condição (not enforcou and not acertou) no while é avaliada a cada iteração do loop. Se a condição for verdadeira, o loop continuará executando. Se a condição for falsa, o loop será interrompido e a mensagem "Fim do jogo" será exibida.

    Dentro do loop, o jogador é solicitado a informar uma letra e a lista de letras acertadas é atualizada com a letra correta, caso o jogador tenha acertado. Se o jogador acertar todas as letras da palavra secreta, a variável acertou será definida como True, encerrando o loop e exibindo a mensagem de "Fim do jogo". Se o jogador errar muitas vezes e a variável enforcou for definida como True, também ocorrerá a mesma coisa, encerrando o loop e exibindo a mensagem de "Fim do jogo".

    > Break = quando executada, encerra o loop naquele ponto. 

3. Funções de String utilizadas:
   >  Upper: utilizada para converter as letras informadas pelo jogador e as letras da palavra secreta em letras maiúsculas, permitindo que a comparação de letras seja feita independentemente se elas foram informadas em maiúsculas ou minúsculas. Isso é importante para evitar erros no jogo, já que as letras maiúsculas e minúsculas são tratadas de forma diferente em Python. Se o jogador informar a letra em minúscula e a letra correta da palavra secreta estiver em maiúscula, a comparação falhará e a letra não será considerada como correta, causando um erro no jogo.

   > Strip: utilizada para remover espaços em branco (ou outros caracteres especificados) no início e fim da string informada pelo jogador no momento em que ele informa uma letra como chute. Essa função é importante para garantir que a entrada do jogador seja válida e para evitar erros no jogo. Se o jogador digitar um espaço ou outro caractere indesejado antes ou depois da letra que ele deseja informar, a função strip() removerá esses caracteres e a comparação da letra informada com as letras da palavra secreta será feita de forma correta.

4. Lista: 
5. Tuplas:
6. Set: coleção não ordenada de elementos. Cada elemento é único, isso significa que não existem elementos duplicados dentro do set.
7. Dictionary: 
