# aula-css
Todas aulas neste repositório -  Criado exclusivamente para fins de armazenamento do meu primeiro curso de HTML . Todos os conteúdos estão nas linhas de código.


No CSS, o símbolo # é usado para selecionar elementos por ID. Cada ID deve ser único dentro de uma página HTML, o que significa que ele só pode ser atribuído a um único elemento. Aqui está um exemplo de como usar o # no CSS. 
o . é classe.

Hover: no css qeur dizer que quando passar o mouse por cima vai exercer alguma função.

TAG DISPLAY {uma das mais importantes do css.
1. DISPLAY: seriam "blocos", como as DIVS que trabalhando como divisorias, display tem o mesmo conceito. 

Display: block = cria blocos

Display:inline = Se ajusta ao espaço somente ocupado dentro da tag. Ex: se eu por uma frase de duas palavras e por a tag display inline
o computador entende que foi ocupado somente duas linhas. 

Display: none = faz desaparecer o bloco
}

POSITION{ Muito usado em imagens com o texto na frente
    position:static; Posicionamento estático, os elementos não podem se mexer, mesmo com comando de direção.
    
    position: relative; Posicionamento relativo,os elementos podem se mexer formando camadas, normalmente usando margens e comando de direção junto. 
        ex: position: relative ;
            left: 40px;
            margin-top: 30px;
            margin left: 20px;
    
    position: fixed; Posicionamento fixa independentemente da rolagem da tela.

    position: absolute; O elemento posicionado com position: absolute se posicionará relativo ao seu ancestral posicionado (com position: relative) mais próximo. Ao encontrar um ancestral posicionado, a posição dos elementos acima dele deixa de ser relevante. 
        por exemplo: div pai e div menores 
            <div class= "pai">
                <div class= "filha1">  </div>
                <div class="filha2">    </div>
            </div>

            .pai{
                position:fixed or relative;
            }
            .filha1, .filha2{
                position:absolute
                bottom: 20; (20px, 20%, ...)
            }
    
    position:sticky; Elemento "gruda" no elemento Pai. em vez dele ficar fixo em relação à tela, ele fica fixo em relação ao rolamento da página. Este tipo de position é utilizado sempre em conjunto das propriedades auxiliares, pois precisa de um posicionamento de referência.
}

OVERFLOW{
    utilizada para tratar conteúdos que ultrapassam os limites de um elemento.O objetivo do overflow é fazer com que conteúdos muito grandes possam caber dentro de uma página através do uso de barras de rolagem. Não funciona sem a propriedade HEIDHT: PX, %, NÚMERO...;
        overflow: visible; Esse é o valor padrão da propriedade overflow, e mostra todo conteúdo que for colocado dentro do elemento, ainda que ultrapasse o tamanho definido.
        div {
            background: green;
             width: 600px;
             height: 210px;
            overflow: visible;
        }
    overflow: hidden; O valor hidden é utilizado quando queremos esconder a parte de um elemento para que ele não passe do tamanho determinado. Geralmente é utilizado junto das propriedades width e height.

    overflow: scroll; ocultando o conteúdo no limite do tamanho definido, porém, ele adiciona também uma barra de rolagem, permitindo acesso ao restante do conteúdo. É importante saber que o valor scroll adicionará barras de rolagem ainda que elas não sejam necessárias.

    overflow: auto; tem o mesmo comportamento do scroll: a única mudança é que o scroll só será adicionado caso seja necessário.

    overflow-x
Essa forma é utilizada para aplicar o overflow apenas na horizontal. Ao fazer isso, a parte vertical assumirá por padrão o valor auto.
overflow-y
Essa forma é utilizada para aplicar o overflow apenas na vertical. Ao fazer isso, a parte horizontal assumirá por padrão o valor auto.
Overflow-x e Overflow-y simplificados
Também é possível replicar o comportamento de overflow-x e overflow-y de forma simplificada utilizando o overflow. Para isso, basta informar 2 valores, o primeiro valor equivale ao overflow-x, já o segundo, equivale ao overflow-y. 
}

Propriedade FLOAT. {
    A propriedade float do CSS é usada para posicionar elementos dentro de um contêiner (DIV QUE ESTA CONTIDA), permitindo que outros elementos se ajustem ao seu redor. Aqui estão os principais valores que você pode usar com a propriedade float:

left: Faz o elemento flutuar à esquerda do contêiner.
right: Faz o elemento flutuar à direita do contêiner.
none: O elemento não flutua, permanecendo no fluxo normal do documento.
inline-start: Flutua o elemento no início da linha, dependendo da direção do texto (esquerda para textos LTR e direita para textos RTL).
inline-end: Flutua o elemento no final da linha, dependendo da direção do texto (direita para textos LTR e esquerda para textos RTL) 
clear: both faz limpar o float
.caixa {
            width: 200px;
            height: 100px;
            margin: 10px;
            border: 1px solid #000;
        }
        .esquerda {
            float: left;
        }
        .direita {
            float: right;
        }
    
}
LIST-STYLE-TYPE{
    propriedade para tirar/mudar o efeito de listas, como text-decoration. 
}

Propriedade OPACITY{
    Serve para fazer efeitos.
    Transforma a imagem/fundo opacos (transparentes), bem dizer. 
    o.1 = 10 porcento de opacidade (muito opaca);
    1.0 = 100 porcento sem opacidade (pouco opaca);
    até chegar ao 1.0, existem vários níveis de opacidade.
}

Propriedade DROPDOWN{
Abre mais opções para selecionar, muito usado em menus
}
 
Importancia no código: 
#ID{}
tag.classe{}
.classe{}
tag{}

efeito gradiente{
    Faz uma imagem degradê.
    comando:
    background-image: linear-gradient(white, blue, black);

    para direcionamento do degrade: 90deg, 180deg, 45 deg (graus)
    ou To left, to right, to top, to bottom right, ...

    background-imagem: radial-gradient (para fazer um circulo de cores)
} 

Sombreado{
    text-shadow: 13px 5px 2px (black) 
    13px=horizontal
    5px=vertical
    2px=intensidade da sombra

    box-shadow: mesmos camandos
}

efeitos de textos{
    letter-spacing: permite controlar o espaço entre as letras do texto.
    line-height: espaçamento entre linhas

    text-overflox: quando o texto passa do tamanho do botão, card, imagem..., ele deixa os 3 pntinhos no final. 
    white-space: é usada para descrever como os espaços em branco dentro dos elementos são manipulados.
    normal
Sequências de espaços em branco são recolhidas. Caracteres de nova linha no código são tratados como outros espaços em branco. As linhas quebram conforme a necessidade para preencher as linhas das caixas (boxes).

nowrap
Recolhe os espaços em branco como no normal, mas suprime as quebras de linha (quebra de texto) no texto.

pre
Sequências de espaço em branco são preservadas, linhas são quebradas apenas em carateres de nova linha no código e em elementos <br>.

pre-wrap
Sequências de espaço em branco são preservadas. Linhas são quebradas em caracteres de nova linha, em <br> e quando necessário para preencher as linhas das caixas (boxes).

pre-line
Sequências de espaços em branco são recolhidas. Linhas são quebradas em caracteres de nova linha, em <br> e quando necessário para preencher as linhas das caixas (boxes).
}
