# Microservicios-APAnaPaula
-----------------------------------------------------------------------------------------------------------
-----------------------------EJERCICIO RETO-CONFIG-SERVICE--------------------------------------------------

1. SEGUIMOS LOS PASOS PROPUESTOS EN CLASE
--MODIFICAR EL POM Y AÑADIRLES LAS DEPENDENCIAS FALTANTES--
--MODIFICAR EL APPLICATION.PROPERTIES A .YML Y AÑADIR LA CONFIGURACIÓN DEPENDIENTE(PUERTO=8085)--
--HACEMOS USO DEL CONFIG-SERVER CREADO DURANTE LA CLASE, Y CREAMOS UN NUEVO RUN CONFIGURATION, 
  AL QUE LE AÑADIMOS UN NUEVO ARGUMENT(-DSERVER.GIT.URI=URL/TO/MY/GIT)----
 --CREAMOS EL CONTROLLER Y MANTENEMOS LOS MISMOS METODOS UTILIZADOS ANTERIORMENTE--
 
 2. ACCEDER--http://localhost:8085/getProductName-----
 
 -------------------------------------------------------------------------------------------------------------
 ---------------------------------EJERCICIO PRICESERVICE-------------------------------------------------------
 
 ERRORES DETECTADOS EN EL EJERCICIO
 1. POM: --CAMBIAR VERSION DE SPRINGBOOT <version>2.6.13</version>---
         --AÑADIR DEPENDENCIA EUREKA CLIENT <dependency>
                                               <groupId>org.springframework.cloud</groupId>
                                               <artifactId>spring-cloud-starter-netflix-eureka-client</artifactId>
		                                         </dependency>
 2. .YML  --AÑADIR PUERTO server: port: 8082-----
          --AÑADIR defaultZone: http://localhost:8761/eureka/----
          
3. PRICE CONTROLLER --CAMBIAR LOS POST X GET--
       
 
