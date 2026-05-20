# Conversor de Monedas

Aplicación de consola desarrollada en **Java** que consume la API de **ExchangeRate** para realizar conversiones en tiempo real entre múltiples divisas. El usuario ingresa el monto y la moneda de origen y destino, y la aplicación retorna el valor equivalente usando la tasa de cambio actual.

Proyecto realizado como parte del programa **Oracle Next Education (ONE) — Alura Latam**.

---

## Tabla de contenidos

- [Descripción](#descripción)
- [Características](#características)
- [Tecnologías](#tecnologías)
- [Requisitos previos](#requisitos-previos)
- [Instalación y configuración](#instalación-y-configuración)
- [Cómo ejecutar el proyecto](#cómo-ejecutar-el-proyecto)
- [Uso](#uso)
- [Contacto](#contacto)

---

## Descripción

Este conversor consulta la API pública de [ExchangeRate](https://www.exchangerate-api.com/) para obtener tasas de cambio actualizadas y permite al usuario convertir cualquier cantidad entre las divisas soportadas. La aplicación funciona desde la consola con un menú interactivo.

El proyecto aplica conceptos clave de desarrollo en Java:

- Consumo de **APIs REST externas** mediante `HttpClient`.
- Mapeo de respuestas JSON a objetos Java con **Gson**.
- Manejo de **variables de entorno** con `Dotenv` para proteger la clave de API.
- Estructuración de un menú interactivo por consola.

## Características

- Conversión en tiempo real entre divisas usando tasas actualizadas.
- Menú interactivo con opciones predefinidas de monedas comunes.
- Gestión segura de la clave de API mediante archivo `.env`.

## Tecnologías

| Categoría | Tecnología |
|---|---|
| Lenguaje | Java |
| API consumida | [ExchangeRate API](https://www.exchangerate-api.com/) |
| Parseo JSON | Gson 2.11.0 |
| Variables de entorno | Dotenv-java 3.1.0 |
| IDE recomendado | IntelliJ IDEA |

## Requisitos previos

- Java JDK 17 o superior
- Una clave de API gratuita de [ExchangeRate API](https://www.exchangerate-api.com/)
- IntelliJ IDEA u otro IDE compatible con Java

## Instalación y configuración

**1. Clonar el repositorio**

```bash
git clone https://github.com/ingArtur/Challenger_Conversor_Moneda.git
cd Challenger_Conversor_Moneda
```

**2. Configurar la clave de API**

Crea un archivo `.env` en la raíz del proyecto con el siguiente contenido:

```
API_KEY=tu_clave_de_exchangerate_aqui
```

> Puedes obtener una clave gratuita registrándote en [exchangerate-api.com](https://www.exchangerate-api.com/).

**3. Verificar las dependencias**

El proyecto incluye las librerías necesarias en formato JAR:

- `gson-2.11.0.jar`
- `dotenv-java-3.1.0.jar`

Asegúrate de tenerlas configuradas como dependencias del proyecto en tu IDE.

## Cómo ejecutar el proyecto

1. Abre el proyecto en **IntelliJ IDEA**.
2. Ubica el archivo `App.java` dentro de `src/com/ChallengerConversorDeMonedas`.
3. Ejecútalo con `Shift + F10` o haciendo clic derecho → **Run 'App'**.

## Uso

Al iniciar la aplicación se muestra un menú con las opciones de conversión disponibles. El usuario:

1. Selecciona el par de divisas a convertir.
2. Ingresa la cantidad.
3. La aplicación consulta la API y muestra el valor equivalente con la tasa actual.

## Contacto

**Artur Andrés Aroca Yara**

- GitHub: [@ingArtur](https://github.com/ingArtur)
- LinkedIn: [Artur Andrés Aroca Yara](https://www.linkedin.com/in/artur-andres-aroca-yara-565363272)
- Email: arthurandres30@gmail.com
