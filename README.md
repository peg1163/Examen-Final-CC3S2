# Examen-Final-CC3S2
## Parte 2 :
### Instalacion de dependecias 
Comenzaremos esta parte del examen ejecutando bundle install para descargar e instalar todas las dependencias :  

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/b8235a63-b280-4bab-b457-0ed84ec77752)  

Las dependencias se instalan correctamente , sin embargo , necesitamos algunas dependencias extras , como faraday y guard para las pruebas , procederemos a incluirlas en nuestro archivo gemfile  

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/5819095a-ea28-433b-84ba-4eaf236a8e36)

y al ejecutar bundle install se logran instalar correctamente :

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/8bb3fe05-8018-4a1a-8080-3e336b1ba520)  

Teniendo ya las dependencias para correr algunas pruebas , crearemos el archivo que controle estas pruebas con rails , con el comando rails generate rspec:install  :


![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/3ff74b51-312b-41c4-80fd-47d5d1fbeafc)  
  
Generados estos archivos , aumentaremos un requerimiento a spec/rails_helper.rb 
, este sera  require 'byebug' 

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/7a0bfc34-3025-46dc-8fc0-5413e9bb9a0f)  

Pasaremos a ejecutar el comando "bundle exec guard init rspec" , al ejecutar dicho comando se nos generara un archivo "Guarfile" lo que nos ayudara a configurar "guard"

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/00ce34b3-8f4b-4d1d-a7f1-53aaa1600b07)  

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/fffc67f6-5378-4934-890e-a45714fa2dfa)

Ya tendriamos listas nuestras dependencias , antes de correr nuestro servidor de manera local , tenemos que hacer la migracion e ingresar los datos que se encuentran en la semilla . 

Ejecutaremos la migracion con el comando "rake db:migrate"

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/12cbd62f-8733-4943-b5fb-375d50423cf9)  

Y cargaremos los datos con "rake db:seed" 

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/c10b27c0-8da4-4210-97d3-b50b4d8952a6)  

Ya tenemos todo listo , ahora podemos ejecutar el servidor de manera local con  " rails server "

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/acc871a9-a952-42f2-805a-53baee2f7548)

ingresaremos a la direccion donde se corre el servidor :

![image](https://github.com/peg1163/Examen-Final-CC3S2/assets/92898224/84be81bb-8eed-41f5-9151-254612bdaa2e)  

### Paso 1 : 




  
