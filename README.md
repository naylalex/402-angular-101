# Instalar ambiente de desarrollo con Angular
https://angular.io/guide/setup-local
Instalar el CLI de Angular
`npm install -g @angular/cli`

No actualizar npm (de momento)

# Crear un espacio de trabajo y una aplicación inicial de Angular
`ng new my-app`
? Would you like to add Angular routing? -> Yes
? Which stylesheet format would you like to use? -> CSS

# Ejecutar la aplicación default
Cambiarse al directorio de la aplicación
`cd my-app`
`ng serve --open`

# hello-world: Crear un componente adicional para la aplicación
`ng generate --help`

Parámetros para el comando ng generate
ng generate component hello-world --dry-run

# Sustituir ruteador default creado por el CLI de Angular
Antes: en @NgModule ()  imports -> AppRoutingModule
Ahora: en @NgModule ()  imports 

RouterModule.forRoot([
    { path: 'hello-world', component: HelloWorldComponent }
])

//TODO: Eliminar encabezado de la aplicación default de Angular

# hello-world-interpolation: Añadir un componente con soporte a interpolación en Angular

Interpolación
```html
<p>{{ message }}</p>
```
 ng generate component hello-world-interpolation --dry-run

 Implementar la interpolación en hello-world-interpolation

 # Implementar un component con NgIf
 `ng generate component hello-world-ngif-component`
