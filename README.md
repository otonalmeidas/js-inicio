![Banner](https://raw.githubusercontent.com/otonalmeidas/js-inicio/master/banner.png)
### Curso gratuito de JavaScript da Rocketseat

Esse curso pertence a trilha Starter da Rocketseat, uma serie de cursos gratuitos de programação como: JavaScript, ES6, NodeJS, ReactJS e React Native.
Para ter acesso, é necessário possuir cadastro no site da Rocketseat, e você pode fazer através <a href="https://app.rocketseat.com.br/signup">deste link</a>.

## <a name="indice">Índice</a>
#### Módulo 1 - Introdução JavaScript
1. [Variáveis e Dados](#aula1)
2. [Operadores Matemáticas](#aula2)
3. [Funções](#aula2)
4. [Condicionais](#aula4)
5. [Operadores Lógicos](#aula5)
6. [Condição Ternária](#aula6)
7. [Estruturas de Repetição](#aula7)
8. [Intervalo e Timeout](#aula8)
9. [Desafios](#desafio1)

#### Módulo 2 - Manipulando a DOM
1. Eventos Inline
2. Trabalhando com a DOM
3. Lidando com Elementos
4. Alterando Estilos
5. Desafio

#### Módulo 3 - App de Todos
1. Estrutura do App
2. Iniciando Aplicação
3. Renderizando Todos
4. Criando Todos
5. Excluindo Todos
6. Salvando no Storage

#### Módulo 4 - JS Assíncrono
1. Requisições AJAX
2. Promises
3. Utilizando Axios
4. Desafio
---
## <a name="aula1">1 - Variáveis e Dados</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula1.png?raw=true" width="600">

[Voltar ao Índice](#indice)

## <a name="aula2">2 - Operações Matemáticas</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula2.png?raw=true" width="450">

[Voltar ao Índice](#indice)

## <a name="aula3">3 - Funções</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula3.png?raw=true" width="505">

[Voltar ao Índice](#indice)

  ## <a name="aula4">4 - Condicionais</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula4.png?raw=true" width="720">

[Voltar ao Índice](#indice)

## <a name="aula5">5 - Operadores Lógicos</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula5.png?raw=true" width="669">

[Voltar ao Índice](#indice)

## <a name="aula6">6 - Condição Ternária</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula6.png?raw=true" width="733">

[Voltar ao Índice](#indice)

## <a name="aula7">7 - Estruturas de Repetição</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula7.png?raw=true" width="510">

[Voltar ao Índice](#indice)

## <a name="aula8">8 - Intervalo e Timeout</a>
<img src="https://github.com/otonalmeidas/js-inicio/blob/master/screenshots/aula8.png?raw=true" width="728">

[Voltar ao Índice](#indice)

## <a name="desafio1">Desafios</a>

### 1 - Crie uma função que dado o objeto a seguir:
```JavaScript
var endereco = {
    rua: "Rua dos pinheiros",
    numero: 1293,
    bairro: "Centro",
    cidade: "São Paulo",
    uf: "SP"
};
```
#### Retorne o seguinte conteúdo:
```
O usuário mora em São Paulo / SP, no bairro Centro, na rua "Rua dos Pinheiros" com nº 1293.
```
#### Resolução:
```JavaScript
function exibeMensagem(endereco) {
    return (
        "O usuário mora em " +
        endereco.cidade +
        " / " +
        endereco.uf +
        ", no bairro " +
        endereco.bairro +
        ', na rua "' +
        endereco.rua +
        '" com nº ' +
        endereco.numero +
        "."
    );
    }
    var endereco = {
        rua: "Rua dos pinheiros",
        numero: 1293,
        bairro: "Centro",
        cidade: "São Paulo",
        uf: "SP"
    };
    console.log(exibeMensagem(endereco));
```
---
### 2 - Crie uma função que dado um intervalo (entre x e y) exiba todos número pares:
```JavaScript
function pares(x,y) {
    // código aqui
}
pares(32, 321);
```
#### Resolução:
```JavaScript
function pares(x, y) {
    for (var i = x; i <= y; i++) {
        if (i % 2 === 0) {
            console.log(i);
        }
    }
}
pares(32, 321);
```
---
### 3 - Escreva uma função que verifique se o vetor de habilidades passado possui a habilidade "Javascript" e retorna um booleano true/false caso exista ou não.
```JavaScript
function temHabilidade(skills) {
    // código aqui
}
var skills = ["Javascript", "ReactJS", "React Native"];
temHabilidade(skills); // true ou false
```
#### Resolução:
```JavaScript
function temHabilidade(skills) {
    return skills.indexOf("Javascript") !== -1;
}
var skills = ["Javascript", "ReactJS", "React Native"];
console.log(temHabilidade(skills));
```
---
### 4 - Escreva uma função que dado um total de anos de estudo retorna o quão experiente o usuário é:
```JavaScript
function experiencia(anos) {
    // código aqui
}
var anosEstudo = 7;
experiencia(anosEstudo);
// De 0-1 ano: Iniciante
// De 1-3 anos: Intermediário
// De 3-6 anos: Avançado
// De 7 acima: Jedi Master
```
#### Resolução:
```JavaScript
function experiencia(anos) {
    if (anos <= 1) {
        return "Iniciante";
    } else if (anos <= 3) {
        return "Intermediário";
    } else if (anos <= 6) {
        return "Avançado";
    } else {
        return "Jedi Master";
    }
}
var anosEstudo = 7;
console.log(experiencia(anosEstudo));
```
---
### 5 - Dado o seguinte vetor de objetos:
```JavaScript
var usuarios = [
    {
        nome: "Diego",
        habilidades: ["Javascript", "ReactJS", "Redux"]
    },
    {
        nome: "Gabriel",
        habilidades: ["VueJS", "Ruby on Rails", "Elixir"]
    }
};
```
#### Escreva uma função que produza o seguinte resultado:
```
O Diego possui as habilidades: Javascript, ReactJS, Redux
O Gabriel possui as habilidades: VueJS, Ruby on Rails, Elixir
```
#### Resolução:
```JavaScript
function exibeHabilidades(usuarios) {
    for (usuario of usuarios) {
        console.log(
        "O " +
        usuario.nome +
        " possui as habilidades: " +
        usuario.habilidades.join(", ")
    );
    }
}
var usuarios = [
{
    nome: "Diego",
    habilidades: ["Javascript", "ReactJS", "Redux"]
},
{
    nome: "Gabriel",
    habilidades: ["VueJS", "Ruby on Rails", "Elixir"]
}
];
exibeHabilidades(usuarios);
```
[Voltar ao Índice](#indice)
