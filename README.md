#include <stdio.h>

int main(){

  printf("   Jogo de Palpites  \n\n Tente adivinhar o numero entre 1 e 50\n\n");
  
  int escolha, palpite;
  int numero_secreto = 29; 
  int jogador = 1;         

  for (;;) { 
    printf("jogador %d digite o seu palpite: ", jogador);
    scanf("%d", &palpite);

    if (palpite == numero_secreto) {
      printf("acertou, o jogador %d ganhou o jogo!\n", jogador);
        break;
    }
    jogador = 3 - jogador;
    printf("errou, passou a vez.\n\n");
  }
    printf("\n Fim de jogo! \n");
}
