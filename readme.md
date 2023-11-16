# Arrays (listas) em JavaScript
Uma lista de conteúdos, como se fosse uma variável que permite diversos valores, inclusive de diversos tipos (string, número, etc).
```
const alunos = ['Maria', 'Joao', 'Daniel', 'Ana'];
```
> A lista de item não inicia como 1, 2, 3, etc. Quem quiser o primeiro item de um array, precisa colocar o numeral zero (0).
```
const alunos = ['Maria', 'Joao', 'Daniel', 'Ana'];

console.log(alunos[0]);
```

### Adicionando e removendo itens
Para **adicionar** um item no array, utiliza-se o termo *push*.
```
const alunos = ['Maria', 'Joao', 'Daniel', 'Ana'];

alunos.push('Renata');
```
ou
```
const alunos = ['Maria', 'Joao', 'Daniel', 'Ana'];

alunos[4] = 'Renata';
```
Para **remover o último item** no array, utiliza-se o termo *pop*.
```
const alunos = ['Maria', 'Joao', 'Daniel', 'Ana'];

console.log(alunos.pop());
```
Para **remover o primeiro item** no array, utiliza-se o termo *shift*.
```
const alunos = ['Maria', 'Joao', 'Daniel', 'Ana'];

console.log(alunos.shift());
```

### Estruturas de repetição
- Para saber o tamanho de um array, utiliza o termo *length*.
```
const alunos = ['Maria', 'Joao', 'Daniel', 'Ana'];

console.log(alunos.length);
```
Para fazer uma operação, como cálculo de média, por exemplo, bastaria depois de utilizar o lenght, pedir para o código somar cada um dos itens indicando suas posições. O problema é que se depois fosse acrescentado outra nota, o código já ficaria inutilizável. **Então como proceder?** Utilizando o laço de repetição **for**.
```
for (let index = 0; index < array.length; index++) {
    const element = array[index]; 
}
```
|Código|Significado|
|------|-----------|
index = 0| interer (índice) é uma variável que vai indicar a partir de que ponto deve começar a realização da operação. Normalmente abrevia, escrevendo apenas a letra i.|
index < array.length| essa parte indica uma estrutura condicional. Enquanto index estiver dentro dos parâmetros desse código, ele será verdadeiro. A partir do momento que se tornar falso, ele parará de executar.|
index++| a terceira e última parte indica o que deve acontecer enquanto o index é verdadeiro. Nesse caso, incrementar mais um.|
dentro das chaves| o código a ser executado enquanto os parâmetros forem verdadeiros.|

