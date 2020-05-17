# CssParser
Solução para um interpretador de css feito em python.

Será utilizado em projetos futuros, em conjunto com o 2JSON


Até o momento, quando o arquivo css é passado para a biblioteca, seus estilos são retornados no formato de lista, sendo o primeiro elemento da lista o nome do estilo e os demais a própria estilização

---

## Exemplo
O seguinte css, quando parseado pelo programa, teria a seguinte saída
##### entrada
<code>
  body {
    background-color: #000;
    font-size: 2rem;
}

/* Comentário */

header {
    color: #fff;
    background-color: #333;
}

/*! Comentário obrigatório */

.header--title {
    font-size: 5rem;
}

.header--box {
    border: 1px solid #efefef
}
</code>
### saída
<code>
>>> cssparser.stylesSheetParser("styles.css")
[['body ', 'background-color: #000', 'font-size: 2rem'], ['header ', 'color: #fff', 'background-color: #333'], ['.header--title ', 'font-size: 5rem'], ['.header--box ', 'border: 1px solid #efefe']]
</code>

## TODO

---

1. Criação da biblioteca 2JSON

