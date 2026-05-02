# Conversor de Unidades (Física)

## Descripción
Script desarrollado para apoyar las prácticas de laboratorio de los estudiantes de la I.E. Simón Bolívar, permitiendo conversiones rápidas entre sistemas de medidas.

## Requisitos Previos
* **Python**: Se requiere **Python 3.10** o superior. No se requieren librerías externas.

## Instalación
Clona el repositorio y accede a la carpeta del proyecto para comenzar:

```
git clone [https://github.com/xxxxx/conversor-fisica-python.git](https://github.com/xxxxx/conversor-fisica-python.git)
cd conversor-fisica-python
```

## Uso
El programa guía al usuario a través de una serie de preguntas en la terminal. Para ejecutarlo:

```
python convertidor_uni.py
```

**Flujo de preguntas:**
1. tipo_medida: Escribe temp para temperatura o dist para distancia.
2. valor_origen: Ingresa el número que deseas convertir.
3. unidad_destino: Selecciona la unidad final (C, F, KM, MI).

**Ejemplo de ejecución:**
> Resultado: 100.00 °C equivalen a 212.00 °F

## Configuración y Parámetros

| Parámetro | Valores permitidos | Descripción |
| :--- | :--- | :--- |
| tipo_medida | temp, dist | Determina el tipo de conversión física. |
| unidad_destino | C, F, KM, MI | Unidades de destino según el tipo de medida. |

**Ajustes de precisión:**
En el código fuente, nosotros podemos modificar la variable DECIMALES_MOSTRADOS. Por defecto es 2, pero puede aumentarse a 4 para cálculos de laboratorio más precisos.

## Manejo de Errores
El sistema detecta automáticamente si el usuario intenta realizar conversiones inválidas:

* **Unidad no reconocida**: Si se ingresa una unidad distinta a las permitidas, el sistema mostrará: [ALERTA] Unidad no reconocida. Usa solo C, F, KM o MI.

## Licencia
Este proyecto educativo se entrega bajo la licencia **MIT**.