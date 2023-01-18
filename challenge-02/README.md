# Desafio da semana #2
.
Nesse exercício, você está livre para escolher os nomes para suas variáveis e funções! :smile:

```js
// Crie uma função que receba dois argumentos e retorne a soma dos mesmos.
?
function soma (x,y){
    return x + y;
}




// Declare uma variável que receba a invocação da função criada acima, passando dois números quaisquer por argumento, e somando `5` ao resultado retornado da função.
?

// Isso foi o que eu escrevi
var loucura = soma;
loucura (5,5) + 5;


//correção 
var loucura = soma( 5, 5 ) + 5;
 

// Qual o valor atualizado dessa variável?
?

15

// Declare uma nova variável, sem valor.
?

var nada = undefined

    //correção
    var nada;


/*
Crie uma função que adicione um valor à variável criada acima, e retorne a string:
    O valor da variável agora é VALOR.
Onde VALOR é o novo valor da variável.
*/
?

// ok estou com dúvida aqui// 
function adiciona_valor (){
    nada = 10;
    return 'O valor da variável agora é ' + nada''
}

// Invoque a função criada acima.
?

adiciona_valor()

// Qual o retorno da função? (Use comentários de bloco).
?

/*
Retorna Agora o valor da variável é 10;
/*


"O valor da variável agora é 10"
/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos;
2. Se qualquer um dos três argumentos não estiverem preenchidos, a função deve retornar a string:
    Preencha todos os valores corretamente!
3. O retorno da função deve ser a multiplicação dos 3 argumentos, somando `2` ao resultado da multiplicação.
*/
?


function blau(x,y,z){
    
    if (x,y,z) {
        return x*y*z + 2;
    }; else {
        return "Preencha todos os valores corretamente!"
    };
    
};


    //Correção
    function blau( a, b, c_){
    if (a === undefined || b === undefined || c === undefined) {
        return "Preencha todos os valores corretamente!"
    }; else {
        return (a * b * c) + 2; 
    };
}    


// Invoque a função criada acima, passando só dois números como argumento.
?

blau(2,4)

// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
?

// "Preencha todos os valores corretamente!"

// Agora invoque novamente a função criada acima, mas passando todos os três argumentos necessários.
?

blau(2,4,5)
// Qual o resultado da invocação acima? (Use comentários para mostrar o valor retornado).
?

//42


/*
Crie uma função com as seguintes características:
1. A função deve receber 3 argumentos.
2. Se somente um argumento for passado, retorne o valor do argumento.
3. Se dois argumentos forem passados, retorne a soma dos dois argumentos.
4. Se todos os argumentos forem passados, retorne a soma do primeiro com o segundo, e o resultado, dividido pelo terceiro.
5. Se nenhum argumento for passado, retorne o valor booleano `false`.
6. E ainda, se nenhuma das condições acima forem atendidas, retorne `null`.
*/
?

function caracter(x,y,z){
    if (x){
        return x;

    } else if (x,y) {
        return x + y;

    } else if (x,y,z) {
        return x+y/z;

    } else if (null) {
        return false 
        
    } else {
        return null
    }


}

// correção (Nunca na vida se usa essa quantidade de else if rsrsr)

funcion threeArgs (x, y, z) {
    if( x !== undefined && y === undefined && z === undefined){ //oq acontece aqui. A instrução só vai ser true quando X for diferente de undefined o Y e o Z não forem passados. Ou seja, X e Y = undefined.

    return x;
    }
    else if (x !== undefined && y !== undefined && z === undefined){ //X e Y foram passados? São diferentes de undefined e Z é undefined, retorna soma X + Y;
        return x + y;
    }
    else if (x !== undefined && y !== undefined && z !== undefined){ 
        return (x + y)/z;
    }
    else if (x === undefined && y === undefined && z === undefined ){
        return false;
    }
    else {
        return null;
    }
}


// Invoque a função acima utilizando todas as possibilidades (com nenhum argumento, com um, com dois e com três.) Coloque um comentário de linha ao lado da função com o resultado de cada invocação.
?

threeArgs(1); // return 1 
threeArgs(5, 3); // return 8
threeArgs(7, 4, 10); // return 1.1
threeArgs(); // return false


