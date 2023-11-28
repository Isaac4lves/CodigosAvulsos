

# CodigosAvulsos

    
Um repositorio onde tem de tudo, desde codigos feitos até finalizados, mas em suma são apenas para diversão e eu não acho que os codigos aqui mereçam um repositorio para eles. Apenas um lugar de diversão com codigos simples...

<br>

<p align="center">
 <img src="https://media0.giphy.com/media/3knKct3fGqxhK/giphy.gif?cid=ecf05e47w498vsbsvlk5z3op5n5mw09as6hildd9cd31k769&ep=v1_gifs_search&rid=giphy.gif&ct=g">
</p>


</div>

<br>

> ### CALCULADORA DE IMC ( C++ )


    #include <iostream>
    #include <string>
    using namespace std;
    
    int main() {
        double peso;
        double altura;
        cout << "insira seu peso\n";
        cin >> peso;
       
       cout << "insira sua altura\n";
       cin >> altura;
       
       double imc = peso/(altura*altura);
       if(imc<=18.5){
           cout << "Abaixo do peso!";
       }
       else if(imc>=18.6 && imc<=24.9){
           cout << "Peso ideal :)";
       }
       else if(imc>=25 && imc<=29.9){
           cout << "Levemente acima do peso...";
       }
       else if(imc>=30 && imc<=34.9){
           cout << "Obesidade grau I";
       }
       else if(imc>=35 && imc<=39.9){
           cout << "Obesidade grau II";
       }
       else{
           cout << "Obesidade Morbida";
       }
    }
    
<br>

> ### PEDRA PAPEL TESOURA ( C++ )
    
    #include <iostream>
    #include <cstdlib>
    using namespace std;
    //0 - pedra, 1 - papel, 2 - tesoura
    int main() {
        
        int jogadaUsuario;
        cout << "0 - Pedra\n1 - Papel\n2 - Tesoura\n -> ";
        cin >> jogadaUsuario;
        
        int jogadaPc=rand()%3;
        
        if(jogadaUsuario==0 && jogadaPc==2){
            cout << "Você Ganhou\nO seu Pc jogou Tesoura e você Pedra e foi derrotado.";
        }
        else if(jogadaUsuario==1 && jogadaPc==0){
            cout << "Você Ganhou\nO seu Pc jogou Pedra e você Papel e foi derrotado.";
        }
        else if(jogadaUsuario==2 && jogadaPc==1){
            cout << "Você Ganhou\nO seu Pc jogou Papel e você Tesoura e foi derrotado.";
        }
        
        else if(jogadaUsuario==0 && jogadaPc==1){
            cout << "Você Perdeu\nO seu Pc jogou Papel e você Pedra e foi vencedor.";
        }
        
        else if(jogadaUsuario==1 && jogadaPc==2){
            cout << "Você Perdeu\nO seu Pc jogou Tesoura e você Papel e foi vencedor.";
        }
        
        else if(jogadaUsuario==2 && jogadaPc==0){
            cout << "Você Perdeu\nO seu Pc jogou Pedra e você Tesoura e foi vencedor.";
        }
        
    
        return 0;
    }
    

  ### ideias de projetos...
  01 - Uma api de compilador para colocar aqui nesse repositorio... <br>
  02 - Sistema de jogo do bixo <br>
  03 - ... <br>
