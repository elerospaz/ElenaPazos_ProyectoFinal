# ElenaPazos_ProyectoFinal
Gestión de inventario - Api Rest con Express
## Instalación

1. Clonar el repositorio
2. Instalar las dependencia

npm install

## Ejecutar el proyecto

npm run start


## Peticiones con Vercel:

-POST  https://elena-pazos-proyecto-final.vercel.app/api/auth/login  
Recibe las credenciales de usuario en el cuerpo (body) de la petición y devuelve el Bearer token si son válidas o un error de autenticación en caso contrario
Credenciales válidas:  {"email":"email@email.com", "password": “password"}

-GET https://elena-pazos-proyecto-final.vercel.app/api/products
Devuelve todos los productos

-GET https://elena-pazos-proyecto-final.vercel.app/api/products/colocarID
Devuelve el producto de ID ingresada

-POST https://elena-pazos-proyecto-final.vercel.app/api/products/create  
Muestra y guarda el producto ingresado en el body (requiere token)

DELETE  https://elena-pazos-proyecto-final.vercel.app/api/products/delete/colocarID 
Elimina el producto de ID ingresada (requiere token)


## Peticiones sin Vercel:

-POST localhost:3000/api/auth/login
Recibe las credenciales de usuario en el cuerpo (body) de la petición y devuelve el Bearer token si son válidas o un error de autenticación en caso contrario.
Credenciales válidas:  {"email":"email@email.com", "password": “password"}

-GET localhost:3000/api/products    
Devuelve todos los productos

-GET localhost:3000/api/products/colocarID
Devuelve el producto de ID ingresada

-POST localhost:3000/api/products/create  
Muestra y guarda el producto ingresado en el body (requiere token)

-DELETE  localhost:3000/api/products/delete/colocarID 
Elimina el producto de ID ingresada (requiere token)




## Variables de entorno:

PORT=3000

FIREBASE_API_KEY=AIzaSyDn-HYCCZPtYFm1OFyJ8kSZP89nUZKrhgE
FIREBASE_AUTH_DOMAIN=gestion-de-inventario-api-rest.firebaseapp.com
FIREBASE_PROJECT_ID=gestion-de-inventario-api-rest
FIREBASE_STORAGE_BUCKET=gestion-de-inventario-api-rest.firebasestorage.app
FIREBASE_MESSAGING_SENDER_ID=611004746207
FIREBASE_APP_ID=1:611004746207:web:930d7c1a910b050dae5c6a

JWT_SECRET=S3cr3T0



