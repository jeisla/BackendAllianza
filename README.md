# BackendAllianza
# PRUEBA TECNICA BACKEND TITA MEDIA

### Configuración
Asegúrate de tener las siguientes herramientas instaladas en tu entorno de desarrollo:
* Java 17
* SringBoot 3.2.0
* Base de datos H2
#### NOTA
Una vez se replique el proyecto, se creo una base de datos en memoria llamada prueba, 
####  La aplicación se ejecutará en http://localhost:8030 por defecto.
Los siguientes Endpoints a ejecutar son:

#### -Crear y guardar clientes.
```bash
  curl --location --request POST 'http://localhost:8030/clients/saveClient'
{
  "name": "John Doe peres robles",
  "phone": "123-456-7890",
  "email": "john.doe@example.com",
  "startDate": "2024-05-25",
  "endDate": "2025-05-25",
  "dataAdded": "2024-05-25"
}
  ```
#### - Listar clientes.
```bash
curl --location --request GET'http://localhost:8030/clients/listClients'
             Body = {"id":1,"sharedKey":"JPeterB","bussinessId":"4274815826419","name":"John Doe peter barrios","phone":"123-456-    
             7890","email":"john.doe@example.com","startDate":"2024-05-25","endDate":"2025-05-25","dataAdded":"2024-05-26"}
  ```
#### - filtrar o buscar clientes.
```bash
curl --location --request GET 'http://localhost:8030/clients/findBySharedKey?sharedKey=JPeteree'
filtro
Objecto
bussinessId: 
"2441743948421"
dataAdded: 
"2024-05-27"
email: 
"pru1@gmail.com"
endDate: 
"2024-05-27"
id: 
1
name: 
"Jesus Alberto Sosa Baron"
phone: 
"3143587960"
sharedKey: 
"JSosaB"
startDate: 
"2024-05-26"
  ```

### Estructura del Proyecto
#### 1. 
  el proyecto o backend esta diseñadopara que nos registre liste y filtre los diferentes clientes que se creen.

