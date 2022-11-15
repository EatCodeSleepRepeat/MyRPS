/*
This ia  rock/paper/scissors/lizard and spock game from
Big Bang Theory.
*/

#include <iostream>
#include <stdlib.h>


int main(){

  srand(time(NULL));

  int computer = rand() %3+1;

  int user = 0;

  std::cout <<"===============================\n";
  std::cout <<"Welcome to Rock Paper Scissors\n";
  std::cout <<"===============================\n";

  std::cout <<"1. Rock\n";
  std::cout <<"2. Paper\n";
  std::cout <<"3. Scissors\n";

  std::cout <<"SHOOT!\n";
  std::cin >> user;

// If computer chooses Rock

  if (computer == 1 && user == 2 ){

   std::cout << "Paper beats rock, you win!";
 
  }

  else if (computer == 1 && user == 3 ){

    std::cout << "Rock beats scissors, you lose!";
  }
  else if (computer == 1 && user == 1){

    std::cout << "It's a draw!";
  }

  // If computer chooses paper

  else if (computer == 2 && user == 1){

    std::cout << "Paper beats rock, you lose!";
  }
  else if (computer == 2 && user == 2){

    std::cout << "It's a draw!";
  }
   else if (computer == 2 && user == 3){

    std::cout << "Scissors beats Paper, you win!";
  }

  // If computer choses Scissors

  else if (computer == 3 && user == 1){

    std::cout << "Rock beats Scissors, you win!";}
    else if (computer == 3 && user == 2){

    std::cout << "Scissors beats paper, you lose!";}
    else if (computer == 3 && user == 3){

    std::cout << "It's a draw!";}
  else {

    std::cout << " Invalid input";
  }

  


}
