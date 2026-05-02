# Generador de Contraseñas Seguras

## Descripción
Módulo de código libre diseñado para que los funcionarios puedan generar contraseñas fuertes y aleatorias directamente desde su terminal, garantizando la seguridad de sus cuentas institucionales.

## Requisitos Previos
* **Node.js**: Es obligatorio tener instalada la versión **v16.0** o superior.
* **Dependencias**: Se utiliza la librería chalk para mejorar la visibilidad de la terminal con colores.

## Instalación
Debido a que el proyecto tiene dependencias externas, es necesario descargar los paquetes antes del primer uso:

```
git clone [https://github.com/xxxxx/generador-pass-node.git](https://github.com/xxxxx/generador-pass-node.git)
cd generador-pass-node
npm install
```

## Uso
El proyecto está configurado con scripts de npm para facilitar su ejecución. Para iniciarlo, utiliza:

```
npm start
```

**Ejemplo de ejecución con parámetros:**
Puedes personalizar la contraseña directamente en el comando:

```
npm start -- --longitud=12 --simbolos=false --numeros=true
```

**Resultado esperado:**
La terminal mostrará en color verde brillante:
> Tu nueva clave es: aB3dE8fG9hI1

## Parámetros de Configuración
Nosotros podemos ajustar la generación mediante las siguientes banderas (flags):

| Parámetro | Tipo | Por defecto | Descripción |
| :--- | :--- | :--- | :--- |
| --longitud | Número | 8 | Longitud de la clave (mín 8, máx 64). |
| --simbolos | Booleano | true | Define si incluye caracteres especiales. |
| --numeros | Booleano | true | Define si incluye números (0-9). |
| --guardar | Flag | N/A | Si se incluye, guarda la clave en mis_claves.txt. |

## Pruebas (Tests)
Para verificar la integridad del generador y asegurar que no hay patrones repetitivos, ejecuta:

npm run test

## Licencia
Este proyecto se distribuye bajo la licencia **MIT**.