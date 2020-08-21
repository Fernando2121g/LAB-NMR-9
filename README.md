EJERCICIO 3
  
precios á"manzana": 2, "naranja": 2.5, "platano": 4, "piña": 3o
mientras que True:
 fruta - input("Dime la fruta que ha vendido: ")
 si fruta.lower() no en precios:
        print("Fruta no existe.")
 Más:
 cantidad á int(input("Dime la cantidad de frutas que vendido: "))
        print("El precio es de %f" % (cantidad * precios[fruta]))
 opcion - input("¡Quieres vender otra fruta (s/n)")
 mientras que opcion.lower() !- "s" y opcion.lower() !- "n":
 opcion - input("¡Quieres vender otra fruta (s/n)")
 si opcion.lower() á "n":
 Romper
 
  EJERCICIO 6
  
  
 archivo de trabajo-open("personas.txt","w")
archivo.write("1; Carlos; Pérez;05/01/1989")
personas["-n2; Manuel; Heredia;26/12/1973","-n3; Rosa; Campos;12/06/1961","-n4;David; García;25/07/2006"]
archivo.writelines(personas)
archivo.close()



de io importación abierta

archivo de archivo á open('personas.txt','r', encoding-"utf8")
lineas - archivo.readlines()
archivo.close()

personas de personas []
para linea en lineas:
 • Borramos los saltos de línea y separamos
 campos á linea.replace("-n", "").split(";") 
 persona á"id":campos[0], "nombre":campos[1], 
 "apellido":campos[2], "nacimiento":campos[3]-
    personas.append(persona)

para p en personas:
 print("(id-) á-> ".format( p['id'], p['nombre'], 
                                         p['apellido'], p['nacimiento']) )
