Proceso CAJA_AUTOMATICA_DE_MEDICAMENTOS
	
	
	Escribir '-----BIENVENIDOS A SOFTPHARMA-----'
	
	
	Escribir "Esta maquina solo acepta billetes de 100,200 y 400"
	
	
	
	
	Escribir 'ESCOJA EL TIPO MEDICAMENTO'
	Escribir "(1)MALESTAR GENERAL. (2) OTROS."
	leer opciones;
	Dimension C[5,8]
	
	definir opinion,dinero,regreso como entero
	opinion=0;
	dinero=0;
	regreso=0;
	Segun opciones Hacer
		1:
			escribir "TIPOS DE MEDICAMENTOS"
			escribir "1) ACETAMINOFEN MK DOP 100 "
			Escribir "2) IBRUPROFENO DOP 100 "
			escribir "3) DOLONEUROBION DOP 200 "
			escribir "4) BRONCOCHEM DOP 400 "
			escribir "5) ALGO DOP 100 "
			leer opion;
			si opion>=1 y opion<=1 entonces 
				escribir 'ingrese su billete '
				leer dinero ;
				si dinero = 100 entonces 
					escribir 'Gracias por su compra'
				sino
					si dinero > 100 entonces 
						regreso= dinero-100;
						escribir 'su devuelta es de :DOP',regreso,' gracias por preferirnos'
						Escribir "1) Volver al menu principal"
				
						leer opciones;
						si opciones>=2 y opciones<=2 entonces
							Escribir 'ESCOJA EL TIPO DE MEDICAMENTO'
							Escribir "(1)MALESTAR GENERAL. (2) OTROS."
							leer opciones;
							escribir "TIPOS DE MEDICAMENTOS"
							escribir "1) ALTRAN800 DOP 100 "
							Escribir "2) OMEPRAZOL DOP 100 "
							escribir "3) ASPIRINA DOP 200 "
							escribir "4) PARACETAMOL DOP 400 "
							escribir "5) INSULINA DOP 400 "
							leer opion;
							
							
						FinSi
					sino 
						escribir "falta dinero";
						
					
					FinSi
				finsi
				
			
			FinSi
			
		2:	escribir "OTROS"
			escribir "1) TE ANTIGRIPAL DOP 100 "
			Escribir "2) LORATADINA DOP 200 "
			escribir "3) SALBUTAMOL DOP 400 "
			leer opion;
			si opciones>=1 y opciones<=1 entonces 
			FinSi
			
				escribir 'ingrese su dinero '
				leer dinero ;
				si dinero = 100 entonces 
					escribir 'Gracias por su compra'
				sino
				FinSi
				
					si dinero > 100 entonces 
						regreso= dinero-100;
						escribir 'su regreso es de :DOP',regreso,' gracias por preferirnos';
					sino 
						escribir "falta dinero";
			
						Finsi
			
		De Otro Modo:
			borrarpantalla;
		Fin Segun
		
	FinProceso
	
