

# CodigosAvulsos

    
Um repositorio onde tem de tudo, desde codigos feitos até finalizados, mas em suma são apenas para diversão e eu não acho que os codigos aqui mereçam um repositorio para eles. Apenas um lugar de diversão com codigos simples...
 Existe um sistema de organização! Cada cor representa um Codigo: <br>
 🔴 -  Simples que foi feito por diversão.<br>
 🔵 -  Simples que pode ser melhorado.<br>
 🟢 -  Que pode ficar mais complexo.<br>
 🟡 -  Que ficou mais complexo.

<br>

<p align="center">
 <img src="https://media0.giphy.com/media/3knKct3fGqxhK/giphy.gif?cid=ecf05e47w498vsbsvlk5z3op5n5mw09as6hildd9cd31k769&ep=v1_gifs_search&rid=giphy.gif&ct=g">
</p>


</div>

<br>

> ### 🔴 CALCULADORA DE IMC ( C++ )


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

> ### 🔴 PEDRA PAPEL TESOURA ( C++ )
    
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
<br>

> ### 🔵 QUANTO SEU CACHORRO COME? ( C++ )
    #include <iostream>
    using namespace std;
    int main() {
        double peso; 
        cout<<"Quanto kilos seu cachorro pesa? "; 
          
        cin>>peso;
           
        if(peso>=1 && peso<=3){
            cout<<"60 gramas por dia! ";
        }
        else if(peso>3 && peso<=5){
            cout<<"de 60 a 85 gramas por dia";
        }
           
        else if(peso>5 && peso<=7){
            cout<<"de 8 a 110 gramas por dia";
        }
           
        else if(peso>7 && peso<=10){
            cout<<"de 110 a 145 gramas por dia";
        }
           
        else if(peso>10 && peso<=25){
            cout<<"de 110 a 145 gramas por dia";
        }
           
        else if(peso>10 && peso<=25){
            cout<<"de 110 a 145 gramas por dia";
        }
           
        else if(peso>25 && peso<=45){
            cout<<"de 110 a 145 gramas por dia";
        }
           
        else if(peso>45 && peso<=60){
            cout<<"de 110 a 145 gramas por dia";
        }
           
        else if(peso>60 && peso<=70){
            cout<<"de 110 a 145 gramas por dia";
        }
        
        else if(peso<1){
            cout<<"💀";
        }
           
        else{
            cout<<"ATOCHA COMIDA NESSA PORRA";
        }
        return 0;
        }          

<br>

> ### 🟢 GERADOR DE DESAFIOS DE PROGRAMAÇÃO. ( Python )
         
    PalavraChave = input("\nFale um assunto para escolhermos um desafio \n-> ")
    LinguagemEscolhida = input("\nLinguagem que deseja usar no codigo \n-> ")
        
    from openai import OpenAI
        
        client = OpenAI(api_key="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")
        chat_completion = client.chat.completions.create(
            messages=[
            {
            "role": "user",
            "content": f"gere um desafio para mim sobre programação a respeito de {PalavraChave} na linguagem de programação {LinguagemEscolhida}.",
            }
            ],
            model="gpt-3.5-turbo",
            )
        print("\n"+chat_completion.choices[0].message.content, 'green')
        
        print("\nPressione Enter para fechar a janela.")
        input()
        
<br>

> ### 🔵 DIGITAL ROOT ( Python )
    a=None
    i=0
    Grelo=0
    print("[numero maximo < 100.000]\n")
    Noom=input("-> ")
    NumRaiz=Noom
    NumRaiz=int(NumRaiz)
    
    
    NumRaiz=str(NumRaiz)
        
    for e in list(NumRaiz) :
        i=i+1
        
    i=i-1
    primeiro = int(NumRaiz[0])
    ultimo = int(NumRaiz[i])
    
        
    if i == 1:
        soma=(primeiro+ultimo)
        print(f"{primeiro}+{ultimo}={soma}")
        
    elif i == 2:
        segundo = int(NumRaiz[1])
        soma=(primeiro+segundo+ultimo)
        print(f"{primeiro}+{segundo}+{ultimo}={soma}")
                
    elif i == 3:
        terceiro = int(NumRaiz[2])
        segundo = int(NumRaiz[1])
        
        soma = (primeiro+segundo+terceiro+ultimo)
        print(f"{primeiro}+{segundo}+{terceiro}+{ultimo}={soma}")
            
    elif i == 4:
        quarto = int(NumRaiz[3])
        terceiro = int(NumRaiz[2])
        segundo = int(NumRaiz[1])
            
        soma = (primeiro+segundo+terceiro+quarto+ultimo)
        print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{ultimo}={soma}")
              
    elif i == 5:
        quinto = int(NumRaiz[4])
        quarto = int(NumRaiz[3])
        terceiro = int(NumRaiz[2])
        segundo = int(NumRaiz[1])
            
        soma = (primeiro+segundo+terceiro+quarto+quinto+ultimo)
        print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{quinto}+{ultimo}={soma}")
          
    elif i == 6:
        sexto = int(NumRaiz[5])
        quinto = int(NumRaiz[4])
        quarto = int(NumRaiz[3])
        terceiro = int(NumRaiz[2])
        segundo = int(NumRaiz[1])
            
        soma = (primeiro+segundo+terceiro+quarto+quinto+sexto+ultimo)
        print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{quinto}+{sexto}+{ultimo}={soma}")
       
            
    if soma>=10:
        soma=str(soma)
        i=0
        
        for f in list(soma) :
            i=i+1
            
        i=i-1
        primeiro = int(soma[0])
        ultimo = int(soma[i])
        
        if i == 1:
            somaII=(primeiro+ultimo)
            print(f"{primeiro}+{ultimo}={somaII}")
            
        elif i == 2:
            segundo = int(soma[1])
            somaII=(primeiro+segundo+ultimo)
            print(f"{primeiro}+{segundo}+{ultimo}={somaII}")
                    
        elif i == 3:
            terceiro = int(soma[2])
            segundo = int(soma[1])
            
            somaII = (primeiro+segundo+terceiro+ultimo)
            print(f"{primeiro}+{segundo}+{terceiro}+{ultimo}={somaII}")
                
        elif i == 4:
            quarto = int(soma[3])
            terceiro = int(soma[2])
            segundo = int(soma[1])
                
            somaII = (primeiro+segundo+terceiro+quarto+ultimo)
            print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{ultimo}={somaII}")  
            
        elif i == 5:
            quinto = int(soma[4])
            quarto = int(soma[3])
            terceiro = int(soma[2])
            segundo = int(soma[1])
                
            somaII = (primeiro+segundo+terceiro+quarto+quinto+ultimo)
            print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{quinto}+{ultimo}={somaII}")
              
        elif i == 6:
            sexto = int(soma[5])
            quinto = int(soma[4])
            quarto = int(soma[3])
            terceiro = int(soma[2])
            segundo = int(soma[1])
                
            somaII = (primeiro+segundo+terceiro+quarto+quinto+sexto+ultimo)
            print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{quinto}+{sexto}+{ultimo}={somaII}")
            
                   
        if somaII>=10:
            somaII=str(somaII)
            i=0
            
            for f in list(somaII) :
                i=i+1
                
            i=i-1
            primeiro = int(somaII[0])
            ultimo = int(somaII[i])
            
            if i == 1:
                somaIII=(primeiro+ultimo)
                print(f"{primeiro}+{ultimo}={somaII}")
                
            elif i == 2:
                segundo = int(somaII[1])
                somaIII=(primeiro+segundo+ultimo)
                print(f"{primeiro}+{segundo}+{ultimo}={somaIII}")
                        
            elif i == 3:
                terceiro = int(somaII[2])
                segundo = int(somaII[1])
                
                somaIII = (primeiro+segundo+terceiro+ultimo)
                print(f"{primeiro}+{segundo}+{terceiro}+{ultimo}={somaIII}")
                    
            elif i == 4:
                quarto = int(somaII[3])
                terceiro = int(somaII[2])
                segundo = int(somaII[1])
                    
                somaIII = (primeiro+segundo+terceiro+quarto+ultimo)
                print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{ultimo}={somaIII}")  
                
            elif i == 5:
                quinto = int(somaII[4])
                quarto = int(somaII[3])
                terceiro = int(somaII[2])
                segundo = int(somaII[1])
                    
                somaIII = (primeiro+segundo+terceiro+quarto+quinto+ultimo)
                print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{quinto}+{ultimo}={somaIII}")
                  
            elif i == 6:
                sexto = int(somaII[5])
                quinto = int(somaII[4])
                quarto = int(somaII[3])
                terceiro = int(somaII[2])
                segundo = int(somaII[1])
                    
                somaIII = (primeiro+segundo+terceiro+quarto+quinto+sexto+ultimo)
                print(f"{primeiro}+{segundo}+{terceiro}+{quarto}+{quinto}+{sexto}+{ultimo}={somaIII}")

  ### ideias de projetos...
  01 - Uma api de compilador para colocar aqui nesse repositorio... <br>
  02 - Sistema de jogo do bixo <br>
  03 - ... <br>
