# animação

<h2>Toda animação precisa de um nome(pode ser qualquer nome)</h2>

animation-name:up;

<h2>Tempo de Duração</h2>

<h3 style="color: #7159c1;">animation-duration: 200ms;</h3>

from: Inicio da animação

to: Fim da animação

@keyframes up{
  from{
    opacity:0;
    trasnform: traslateY(15px) ( EIXO Y: &uarr; &darr;)
}
to{
  opacity:1;
}

*obs: ele vai voltar a posição normal após a animação

<h2>para ele não voltar no padrão e ficar no 'to(do keyframes)', use isso:</h2>

animation-fill-mode: forwards;//fica no 'to'
animation-fill-mode: backwards;//voltar para posição padrão

*proximo recomendado para Javascript , para quando clicar em algum botão
animation-play-state:paused; após use running

<h2>-faz tudo ao contrário do que foi pedido</h2>
animation-direction: reverse;

animation-iteration-count:infinite; //roda infinito

<h2>MAS TUDO PODE SER SIMPLIFICADO ASSIM:</h2>
animation : up 200ms ease-out;
            nome , tempo, tipo de entrada (se é suave ou não)

