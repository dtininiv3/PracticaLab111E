# Practica Lab-111E


print('----------------------------------')
print('Usuario                          usuario:Daniel         contraseña:12345')
print('----------------------------------')
n=input('Ingrese su nombre de usuario:')
c=int(input('Ingrese su contraseña:'))
if (n == 'Daniel' and c==12345):
        
				print ('Incio Sesion')
				def pedirNumeroEntero():
				
				    correcto=False
				    num=0
				    while(not correcto):
				        try:
				            num = int(input("Introduce una Opcion: "))
				            correcto=True
				        except ValueError:
				            print('Error, Introduce un numero entero.')
				    
				    return num
				
				salir = False
				opcion = 0
				
				while not salir:
				
				    print ("1.Division de 2 Numeros.")
				    print ("2.Divisores.")
				    print ("3.Numeros Capicua.")
				    print ("3.Cambio de Base.")
				    print ("5.Salir")
					
				    opcion = pedirNumeroEntero()
				
				    if opcion == 1:
				        print ("1.Primera Operacion")
				        
				        a=int(input("Ingresa un primer numero:"))
				        b=int(input("Ingresa un segundo numero:"))
				        dre=a//b
				        print(dre)
				        
				    elif opcion == 2:
				        print ("2.Segunda Operacion")  	
				        c=int(input("Ingresa un numero:"))
				        if c > 99999999999999:
				        	print("Divisor de",c,"son:")
				        	for i in range(1,c+1):
				        		if c % i == 0:
				        			print(i,end=" ")  
				        			print()
				        else:
				        	print("Numeros mayores a 99999999999999.")
				        	    		   	   	
				    elif opcion == 3:
				        print ("3.Tercera Operacion")
				        d=int(input("Ingrese un n termino:"))
				        if d > 99999999:
				        	
				        	al=10
				        	ct=0
				        	for f in range(al,d+1):
				        		num_s=str(f)
				        		num_list=list(num_s)
				        		if num_list==num_list[::-1]:
				        			cap=''.join(num_list)
				        			ct+=1
				        			print(cap)
				        	print("Total capicuas",ct)
				        else:
				        	print("Ingrese numerors mayores a 99999999")
				    elif opcion == 4:
				        print ("4.Cuarta Operacion")
				        
				        e=int(input("Ingresa un numero:"))
				        x=int(input("Ingresa la base:"))
				        print(e,"^",x)
				        resdec=e / 10
				        print("Convertido a decimal, invertido es:")
				        total=resdec ** x
				        rtotal=x**e
				        print(rtotal)    
				        
				    elif opcion == 5:
				        salir = True
				    else:
				        print ("Introduce un numero entre 1 y 5")
				
				print ("Fin")

else:
	print("Hubo un error en la Contraseña")
