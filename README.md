salbrEX = float(input("Digite o valor do salário: "))


#Vale Transporte

if salbrEX <= 1320:

    descINSS = 7.5

    descINSSv1 = (salbrEX/100)*descINSS

    final1 = salbrEX - descINSSv1

    print (f"Valor do Desconto do INSS: {descINSSv1}")


elif salbrEX > 1320 and salbrEX <= 2571.29:

    descINSS = 9.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (salbrEX - 1320)/100*9.0

    final1 = salbrEX - descINSSv1 - descINSSv2 - 19.80

    print (f"Valor do Desconto do INSS: {descINSSv1}, {descINSSv2}")


elif salbrEX > 2571.29 and salbrEX <= 3856.94:

    descINSS = 12.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (2571.29 - 1320)/100*9.0

    descINSSv3 = (salbrEX - 2571.29)/100*12.0

    final1 = salbrEX - (descINSSv1 + descINSSv2 + descINSSv3 + 96.94)

    print (f"Valor do Desconto do INSS: {descINSSv1}, {descINSSv2}, {descINSSv3}")


elif salbrEX > 3856.94 and salbrEX < 7507.49:

    descINSS = 14.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (2571.29 - 1320)/100*9.0

    descINSSv3 = (3856.94 - 2571.29)/100*12.0

    descINSSv4 = (salbrEX - 3856.94)/100*14.0

    final1 = salbrEX - descINSSv1 - descINSSv2 - descINSSv3 - descINSSv4 - 174.08

    print (f"Valor do Desconto do INSS: {descINSSv1}, {descINSSv2}, {descINSSv3}, {descINSSv4}")


elif salbrEX > 7507.49:

    descINSS = 14.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (2571.29 - 1320)/100*9.0

    descINSSv3 = (3856.94 - 2571.29)/100*12.0

    descINSSv4 = (salbrEX - 3856.94)/100*14.0

    final1 = salbrEX - descINSSv1 - descINSSv2 - descINSSv3 - descINSSv4 - 876.95

    print (f"Valor do Desconto do INSS: {descINSSv1}, {descINSSv2}, {descINSSv3}, {descINSSv4}")

 

 

#Sem Vale Transporte 

if salbrEX <= 1320:

    descVT = (salbrEX/100)*6.0

    descINSS = 7.5

    descINSSv1 = (salbrEX/100)*descINSS

    final2 = salbrEX - (descINSSv1 + descVT)

    print (f"Valor do Desconto do Vale Transporte: {descVT}")


elif salbrEX > 1320 and salbrEX <= 2571.29:

    descVT = (salbrEX/100)*6.0

    descINSS = 9.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (salbrEX - 1320)/100*9.0

    final2 = salbrEX - (descINSSv1 + descINSSv2 + descVT + 19.80)

    print (f"Valor do Desconto do Vale Transporte: {descVT}")


elif salbrEX > 2571.29 and salbrEX <= 3856.94:

    descVT = (salbrEX/100)*6.0

    descINSS = 12.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (2571.29 - 1320)/100*9.0

    descINSSv3 = (salbrEX - 2571.29)/100*12.0

    final2 = salbrEX - (descINSSv1 + descINSSv2 + descINSSv3 + descVT + 96.94)

    print (f"Valor do Desconto do Vale Transporte: {descVT}")


elif salbrEX > 3856.94 and salbrEX < 7507.49:

    descVT = (salbrEX/100)*6.0

    descINSS = 14.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (2571.29 - 1320)/100*9.0

    descINSSv3 = (3856.94 - 2571.29)/100*12.0

    descINSSv4 = (salbrEX - 3856.94)/100*14.0

    final2 = salbrEX - (descINSSv1 + descINSSv2 + descINSSv3 + descINSSv4 + descVT + 174.08)

    print (f"Valor do Desconto do Vale Transporte: {descVT}")


elif salbrEX > 7507.49:

    descVT = (salbrEX/100)*6.0

    descINSS = 14.0

    descINSSv1 =  (1320/100)*7.5

    descINSSv2 = (2571.29 - 1320)/100*9.0

    descINSSv3 = (3856.94 - 2571.29)/100*12.0

    descINSSv4 = (salbrEX - 3856.94)/100*14.0

    final2 = salbrEX - (descINSSv1 + descINSSv2 + descINSSv3 + descINSSv4 + descVT + 876.95)

    print (f"Valor do Desconto do Vale Transporte: {descVT}")



VT = input ("Descontar Vale Transporte do Salário?: ")

if VT == "s":

 print (f"Salário final com desconto do INSS e Vale Transporte:{final2}")

 print (f"Salário Líquido: {final2}")

elif VT:

 print (f"Salário final com desconto do INSS:{final1}")

 print (f"Salário Líquido: {final1}")
