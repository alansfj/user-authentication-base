
# Setup development:

## Backend:

1. Entra a la carpeta backend
2. Ejecutar el comando ```npm i```
3. Copia el contenido del archivo .env.template y pegar su contenido en un nuevo archivo llamado .env
4. Inicia docker y ejecutar el comando ```docker compose up -d```
5. Ejecutar el comando ```npm run dev```

## Migraciones:
1. Para crear una migracion se ejecuta el comando ```npm run pg-migration create {{migration-name}}```
2. Se modifica el archivo de la migracion creada y se guarda
3. Se ejecuta el comando ```npm run pg-migration up``` o ```npm run pg-migration down``` segun la migracion
4. Cada que se ejecute una migracion es importante ejecutar el comando ```npm run kysely-codegen``` 
para que kysely genere los tipos