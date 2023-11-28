# CodigosAvulsos
Um repositorio onde tem de tudo, desde codigos feitos até finalizados. Uma bagunça...


> ### CALCULADORA DE IMC
    C++ ->


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

    

  ### ideias de projetos...
  01 - Uma api de compilador para colocar aqui nesse repositorio... <br>
  02 - Sistema de jogo do bixo <br>
  03 - ... <br>
