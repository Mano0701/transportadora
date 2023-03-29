# transportadora
visualg
Algoritmo "Transportadora"
// Disciplina   : [Linguagem e Lógica de Programação]
// Professor   : NEIVA
// Descrição   : Calcular Frete
// Autor(a)    : Ismael.F.Dinnebier
// Data atual  : 28/03/2023
Var
nome,endereco,bairro,cidade,estado : caractere
nome1,endereco1,bairro1,cidade1,estado1 : caractere
val_tot,peso_bruto,valor_seg,trans_imp:real
cd,CEP,CEP1:Inteiro
seguro: logico

Inicio
   Escreval("-----------------------------------------------")
   Escreval("|                TRANSPORTES RS               |")
   Escreval("-----------------------------------------------")
   Escreval("Preencha os dados do remetente!")
   Escreval("Nome: ")
    Leia(nome)
   Escreval("Endereco: ")
    Leia(Endereco)
   Escreval("bairro")
    Leia(bairro)
   Escreval("CEP")
    Leia(CEP)
   Escreval("cidade")
    Leia(cidade)
   Escreval("estado")
    Leia(estado)
     LimpaTela
   Escreval("-----------------------------------------------")
   Escreval("|                TRANSPORTES RS               |")
   Escreval("-----------------------------------------------")
   Escreval("Preencha os dados do destinatário!")
   Escreval("Nome: ")
    Leia(nome1)
   Escreval("Endereco: ")
    Leia(Endereco1)
   Escreval("bairro")
    Leia(bairro)
   Escreval("CEP")
    Leia(CEP1)
   Escreval("cidade")
    Leia(cidade1)
   Escreval("estado")
    Leia(estado1)
   Escreval("Digite o valor total dos produtos")
    Leia(val_tot)
   Escreval("Qual o peso total dos produtos?")
    Leia(peso_bruto)
     LimpaTela
   Escreval("-----------------------------------------------")
   Escreval("|                TRANSPORTES RS               |")
   Escreval("-----------------------------------------------")
   Escreval("[1]Norte 20,00R$ po Kg")
   Escreval("[2]Sul 18,00R$ po Kg")
   Escreval("[3]Nordeste 19,00R$ po Kg")
   Escreval("[4]Sudoeste 17,00R$ po Kg")
   Escreval("[5]Centro-Oeste 10,00R$ po Kg")
   Escreva("Qual seu codigo de destino: ")
   Escreval("____________________________")
    Leia(cd)
     Se (cd = 1) entao
      peso_bruto <- (peso_bruto * 20)
       SeNao
        Se (cd = 2) entao
         peso_bruto <- (peso_bruto * 18)
          SeNao
           Se (cd = 3) entao
            peso_bruto <- (peso_bruto * 17)
             SeNao
              Se (cd = 4) entao
               peso_bruto <- (peso_bruto * 10)
                SeNao
                 Se (cd >= 5) entao
                  Escreval ("!!Destino Inexistente!!")
                 FimSe
              FimSe
           FimSe
        FimSe
     FimSe
   Escreval("Gostaria de adicionar o seguro?")
   Escreval("Digite [s] para aceitar!")
   Escreval("Digite [n] para negar!")
     Leia(seguro)
     Se (seguro = s) entao
       valor_seg <- ((val_tot*20)/100)
      Senao
       valor_seg <- (0)
     FimSe
       trans_imp <- (valor_seg + val_tot + peso_bruto)
      LimpaTela
   Escreval("-----------------------------------------------")
   Escreval("|                TRANSPORTES RS               |")
   Escreval("-----------------------------------------------")
   Escreval("  ")
   Escreval("O TRANSPORTE DE",nome".")
   Escreval("O transporte de",peso_bruto," R$")
   Escreval("Para ",nome1,"de ",Endereco1,
   
       
       
Fimalgoritmo
