<?php

echo "Seja bem-vindo ao jogo de CARA ou COROA\n";

$nomeJogador = readline("Identifique-se:");

echo "Olá {$nomeJogador}, você escolhe CARA ou COROA?\n";

echo $escolhaJogador;

do{
  $escolhaJogador = (int) readline("Digite 0 para CARA e 1 para COROA: ");
}while($escolhaJogador !== 0 && $escolhaJogador !==1);

$sorteio = rand(0,1);

if($escolhaJogador===$sorteio){
  echo "Parabéns! Você venceu!";
}
else{
  echo "Uhhhuuuuu! Eu venci você!";
}