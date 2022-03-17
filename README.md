# Exerc-cio-JavaScript
Obtenha dados da altura e o sexo (M ou F) de 15 pessoas e apresente os seguintes resultados:  - A maior e a menor altura do grupo; - A média de altura dos homens; - O número de mulheres.
var i, altura, sexo, maioralt = 0, menoralt = 0, hom = 0, mulh = 0, mediamulh = 0, contamulh = 0, contahom = 0;

            for(i = 1 ;i <= 15; i++) {        
                altura = parseInt(prompt("Informe sua altura["+i+"]:"));
                sexo = prompt("Sexo: M ou F:");


                if(i == 1) {
                    menoralt = altura;
                } if(altura > maioralt) { 
                    maioralt = altura;
                } if(altura < menoralt) { 
                    menoralt = altura;
                } if(sexo == 'M') {
                    hom += altura;
                    contahom++;
                } else if(sexo == 'F') {
                    mulh += altura;
                    contamulh++;
                }
            }
            mediahom = hom/contahom;
            alert("A maior altura é: "+maioralt); 
            alert("A menor altura é: "+menoralt);
            alert("A média dos homens é: "+mediahom);
            alert("O número de mulheres é: "+contamulh);
