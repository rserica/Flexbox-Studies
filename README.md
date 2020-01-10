# Studies-Flex-CSS


# CONTAINER PROPERTIES
## FLEX-DIRECTION
    A propriedade **flex-direction** aceita basicamente quatro propriedades.
      flex-direction: row | row-reverse | column | column-reverse;
### ROW
    - É a propriedade default do flex, ele alinha o layout em linhas, ou seja suas divs ficarão encaixadas numa unica linha.

### ROW REVERSE
    - É a mesma coisa que a row, a diferença é que esta propriedade organiza suas divs de trás pra frente.

### COLUMN
  - Alinha o layout em coluna, ou seja, os items ficarão organizados encaixados em varias linhas com uma ou mais colunas.

### COLUMN REVERSE
      - É a mesma coisa que a COLUMN, a diferença é que esta propriedade organiza suas divs de trás pra frente.

## FLEX-WRAP
      Determina se os elementos filhos que estão dentro do container irão aceitar ou não a quebra do conteudo.
      flex-wrap: nowrap | wrap | wrap-reverse

### NOWRAP
    - É o default desta propriedade, todos os flex-items ficarão sempre na mesma linha.

### WRAP
    Os items irão se encaixar em diversas linhas de acordo com o seu tamanho.
    Exempo: Se eu tenho um layout com a largura de 500px e tenho items com a largura de 220 pixels, esses items vão se encaixar em colunas até o tamanho maximo e se quebrar para continuar na outra linha

### WRAP-REVERSE
    Os items flex irão se encaixar em multiplas linhas porem de baixo para cima.

## FLEX-FLOW
    É uma propriedade que engloba o flex-wrap e o flex-direction em uma propriedade só

    flex-flow: FLEX-WRAP || FLEX-DIRECTION;

## JUSTIFY-CONTENT
    É a propriedade que define o alinhamento no eixo X
    justify-content: flex-start | flex-end | space-between | space-around | space evenly | center

### FLEX-START
    Os items são colocados no começo da direção do flex
### FLEX-END
    Os items são colocados no fim da direção do flex
### CENTER
    Os items são colocados no centro
### SPACE-AROUND
    Ele gera espacos proporcionais ao tamanho dos elementos.
### SPACE-BETWEEN
    Os items são distribuidos na linha, primeiros items no começo e os ultimso items no final. A distribuição começa do centro para as extremidades  
### SPACE-EVENLY
    Os items sao distribuidos de modo que tenha um espaco igual entre os items

**Algumas dessas propriedades não sao suportadas pelos navegadores, portanto o mais seguro é usar flex-start , flex-end e center**

## ALIGN CONTENT
  É a propriedade que define o alinhamento no eixo X
  align-content: flex-start | flex-end | space-between | space-around | space evenly | center | stretch
### STRETCH
    É a propriedade que estica o item até a altura total da flex-row
### BASELINE
    O item vai ficar da altura do conteudo que está dentro.

  **Possui as mesmas propriedades do justify content**

#ITEM PROPERTIES
## ORDER
    Os items por defaut são ordenados de acordo com a ordem em que eles são criados. Porém, é possivel

    order: <integer>;
## FLEX-GROW
    Esta propriedade atribui ao item a habilidade de crescer, se necessário. Ele define a quantidade de espaço disponivel dentro de um flex-container um item pode tomar pra si.

    Se todos os items tem flex-grow:1, o espaço restante vai ser distribuido igualmente entre os items. Se um dos items tem flex-grow:2, ele vai tomar duas vezes mais espaço.

## FLEX-SHRINK
    Se comporta de maneira semelhante porém contraria ao flex-grow, ao inves de expandir, ele encolhe.


## FLEXBASIS
    Define o tamano default de um elemento antes de o espaço restante ser distribuido. Pode ser um tamanho ou uma palavra-chave.

    flex-basis: <lenght> || auto;

## FLEX
    É uma propriedade combo que junta flex-grow, flex-shrink e flex-basis.

    flex: <flex-grow> <flex-shrink> <flex-base>

## ALIGN-SELF
    Funciona semelhante ao **align-items** porém para items unicos.

    align-self: auto | flex-start | flex-end | center | baseline | stretch;


## Links Úteis
Official Guide to Flexbox: https://www.w3.org/TR/css-flexbox-1/
Compatibilidade com outros navegadores: https://autoprefixer.github.io/
Can I use Flexbox?: https://caniuse.com/#search=flex-box
Another Flexbox Playground: https://demos.scotch.io/visual-guide-to-css3-flexbox-flexbox-playground/demos/
Flexbox Playground: https://codepen.io/enxaneta/full/adLPwv
A guide to Flexbox: https://css-tricks.com/snippets/css/a-guide-to-flexbox/#flexbox-background
