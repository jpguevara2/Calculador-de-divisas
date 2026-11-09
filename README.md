# 💱 Calculador de Divisas (API Integration)

Aplicación web/móvil diseñada para realizar conversiones de moneda en tiempo real, conectándose a una API REST externa para obtener tasas de cambio actualizadas de forma dinámica.

![image](https://user-images.githubusercontent.com/45580750/222188377-2f935574-519a-4433-8983-b26cb968fe55.png)


## 🎯 Problema y Solución

* **El Problema:** Las tasas de cambio entre divisas varían constantemente. Utilizar valores estáticos o realizar cálculos manuales genera datos desactualizados e imprecisos para transacciones o presupuestos.
* **La Solución:** Una herramienta interactiva que consume un servicio web externo (API) para consultar los valores oficiales del mercado en tiempo real, procesar la conversión de forma automática y entregar resultados precisos al usuario.

## ⚙️ Funcionalidades Clave e Integración

* **Consumo de API REST en Tiempo Real:** Conexión asíncrona a servicio web externo para la sincronización automática de las divisas y sus equivalencias.
* **Procesamiento de Respuestas JSON:** Parseo y extracción dinámica de los datos de tasas de cambio recibidos desde el servidor.
* **Conversión y Formato Financiero:** Cálculo instantáneo del monto final aplicando la tasa vigente y redondeo decimal adecuado para precisión monetaria.
* **Manejo de Errores y Validaciones:** Control de excepciones ante fallas de red, problemas de conexión con la API o datos de entrada inválidos por parte del usuario.

## 🛠️ Aspectos Técnicos y Arquitectura

* **Protocolo de Comunicación:** HTTP Client (`fetch` / `axios` / `HttpURLConnection` según el lenguaje utilizado) para consumo de API REST.
* **Formato de Datos:** JSON (JavaScript Object Notation).
* **Manejo de Asincronía:** Uso de promesas (`Promises` / `async-await`) para garantizar que la interfaz no se bloquee mientras se realiza la consulta remota.
* **Sanitización de Entradas:** Filtrado de datos ingresados para prevenir errores numéricos en la interfaz.
