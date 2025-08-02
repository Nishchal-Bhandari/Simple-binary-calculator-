# Simple-binary-calculator-
print("\t\t\tSIMPLE CALCULATOR \n\n")
print("This is a binary calculator💻. you can perform binary operations using it.\n")
print("Note:\n   \t you can perform +,-,×,÷\n")
print(".........................................")

equ=input()

mlen=len(equ)
elen=len(equ)-1  

if (equ[mlen-1])=="=":
   if ("+"in equ)==True:
     opn="+"
   elif ("-"in equ)==True:
       opn="-"
   elif ("×"in equ)==True:
       opn="×"
   elif ("÷"in equ)==True:
       opn="÷"
   else:
        print("INVALID OPERATION 😭 ")
        exit()
    

   for i in range(elen):
       if equ[i]==opn:
         loc=i

   opd1=int(equ[0:loc])
   opd2=int(equ[loc+1:mlen-1])


   if opn=="+":
      res=opd1+opd2
   elif opn=="-":
       res=opd1-opd2
   elif opn=="×":
       res=opd1*opd2
   elif opn=="÷":
       res=opd1/opd2
    
    
   print(res)

else:
    print("INVALID OPERATION 😭 ")
print("heelo")


hello this is a simple calculater