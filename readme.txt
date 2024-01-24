#Instrucciones para la ejecución del proyecto:

PRE REQUISITOS:
-Tener instalado IntelliJ IDEA, de preferencia en su ultima version.
-Tener Instalado y Configurado Java 8 u 11
-Tener Instalado Maven
-Contar con los Plugins de Cucumber for Java y Gherkin

PASOS PARA LA EJECUCIÓN:
1- Colocar en el RunnerTest.java, en la linea: return Karate.run("classpath:(UBICACIÓN DEL ARCHIVO FEATURE). 
	Ejemplo:
		return Karate.run("classpath:bdd/Features/PetStore.feature")

2- Colocar en el RunnerTest.java el tag correspondiente. (@PostPet). (PARA LO SOLICITADO SE RECOMIENDA PRIMERO EJECUTAR EL TAG @PostPet Y LUEGO EL TAG GENERAL)

3- Para la validación completa de lo solicitado, se recomienda en una segunda ejecución enviar el tag general para los demás Scenarios. 
	Para ello solo se cambia el tag @PostPet por el tag @PetStore

3- Luego de tener listos los pasos 1 y 2 puede ejecutarse el "Run" del "RunnerTestCert"

PASOS PARA LA VALIDACIÓN DE RESULTADOS:
- Se puede validar los resultados al finalizar la ejecución. Deberia indicar resultado 200 en cada ejecución.
- Se puede visualizar la evidencia de la ejecución colocando la siguiente ruta en el navegador de su preferencia:
	C:\Proyectos\Challenge_QA_APIs\target\karate-reports\karate-summary.html


