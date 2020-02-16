# animação

Toda animação precisa de um nome(pode ser qualquer nome)

animation-name:up;

Tempo de Duração

animation-duration: 200ms;

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

para ele não voltar no padrão e ficar no 'to(do keyframes)', use isso

animation-fill-mode: forwards;//fica no 'to'
animation-fill-mode: backwards;//voltar para posição padrão

*proximo recomendado para Javascript , para quando clicar em algum botão
animation-play-state:paused; após use running

-faz tudo ao contrário do que foi pedido
animation-direction: reverse;

animation-iteration-count:infinite; //roda infinito

MAS TUDO PODE SER SIMPLIFICADO ASSIM:
animation : up 200ms ease-out;
            nome , tempo, tipo de entrada (se é suave ou não)

