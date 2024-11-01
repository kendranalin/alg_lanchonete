# alg_lanchonete
algoritmo lanchonete
Algoritmo "lanchonete"
alterando branch
Var

  ql,qb,b:inteiro // ql=quantidade de lanche, qb=quantidade de bebidas

  VL,VB,VTC,T,p,f,vp:real // VTC=valor total da compra, VL=valor lanches
  // VB=bebidas, T=troco, p=pagamento, f=falta dinheiro/  vp= valor pago

  la,bd,pl,pb:real // la=lanches, bd=bebidas, pl=preço lanche, pb=preço bebidas

  oplanche, opbebida:caracter // oplanche=opção lanche, opbebidas=opção de bebidas

Inicio

    escreval("Deseja comprar um lanche? sim/não")
    leia(oplanche)

    se (oplanche="s") entao
       escreval("Lanches")
       escreval("1 - X Salada.................R$ 12,00")
       escreval("2 - Hambúrguer Simples.......R$ 10,00")
       escreval("3 - Hambúrguer Duplo.........R$ 14,00")
       escreval("4 - X Egg....................R$ 13,50")
       escreval("5 - X Tudo...................R$ 15,50")
       escreval("DIGITE O NÚMERO E COM O LANCHE ESCOLHIDO")
       leia(la)


       escolha la
            caso 1
               pl:=12
            caso 2
               pl:=10
            caso 3
               pl:=14
            caso 4
               pl:=13.50
            caso 5
               pl:=15.50
            outrocaso
               escreval("Lanche inválido")
       fimescolha

       escreval("QUANTIDADE")
       leia(ql)

       VL:=ql*pl
    fimse

    escreval("Valor total do lanche R$ ",VL:2:2," reais")


    escreval ("deseja escolher uma bebida? sim/não")
    leia (opbebida)
    se (opbebida="s") entao

    escreval("bebidas")
    escreval("11 - Refringente..........................R$ 9,50")
    escreval("12 - Suco de laranja.....................R$ 10,88")
    escreval("13 - Água mineral com gás.................R$ 5,50")
    escreval("14 - Água mineral sem gás.................R$ 9,80")
    escreval("15 - Suco de uva.........................R$ 10,50")

    escreval ("digite o numero e com a bebida escolhida")
    leia (b)

    escolha b

    caso 11
    pb:= 9.50

    caso 12
    pb:= 10.88

    caso 13
    pb:= 5.50

    caso 14
    pb:= 9.80

    caso 15
    pb:= 10.50

    outrocaso
     escreval ("bebida invalida")
    fimescolha

    escreval("QUANTIDADE DE BEBIDAS")
       leia(qb)

    VB:=qb*pb
    fimse
     escreval("Valor da bebida R$ ",VB:2:2," reais")
     
     
    VTC:=VL+VB
     
    escreval ("informe o valor pago")
    leia (vp)
    
    
    
    se (vp<VTC) entao
    escreval("Pagamento insuficiente")
    
    
       fimse


Fimalgoritmo
