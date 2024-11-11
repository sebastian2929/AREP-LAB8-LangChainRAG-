# Lang Chain RAG

Este proyecto utiliza la biblioteca LangChain para desarrollar una aplicación que implementa una Recuperación Asistida por Generación (RAG), optimizando la integración y recuperación de información mediante modelos de lenguaje. A continuación, se describen los detalles de su arquitectura y componentes, así como las instrucciones para instalar y ejecutar el proyecto.

## Arquitectura y Componentes

El notebook sigue una estructura modular y comprende los siguientes componentes principales:

**1.**  **Instalación de Librerías:** Se actualizan e instalan las librerías langchain, langchain-community, y langchain-chroma para asegurar compatibilidad y acceso a las últimas funcionalidades de LangChain.

**2.** **Configuración de Variables de Entorno:**
- Se configura la variable LANGCHAIN_TRACING_V2 para habilitar el seguimiento avanzado.
- LANGCHAIN_API_KEY: Permite establecer la clave API del usuario para acceder a funciones de LangChain. Esta clave se ingresa mediante el módulo getpass, garantizando que se mantenga segura.

**3.** **Implementación y Configuración de RAG:** El núcleo del notebook incluye configuraciones avanzadas para la recuperación de información utilizando LangChain. La implementación específica puede incluir pasos para cargar datos, crear una base de conocimiento o indexación, y optimizar el acceso a través de consultas de lenguaje natural.

![image](https://github.com/user-attachments/assets/b1b80e09-21ab-4838-a193-e4989c2b1b74)


## Instalación y Ejecución
Sigue los siguientes pasos para instalar las dependencias y ejecutar el proyecto en un entorno de Jupyter Notebook:

**1.** **Clonar el repositorio:**
``` 
git clone https://github.com/sebastian2929/AREP-LAB8-LangChainRAG-.git

cd LangChainRAG
```
**2. Instalar dependencias:**
Abre el archivo LangChainRAG.ipynb en Jupyter Notebook y ejecuta las primeras celdas. La instalación de dependencias es automática e incluye:
```
%pip install --quiet --upgrade langchain langchain-community langchain-chroma
```

**3. Configurar las variables de entorno:**
Asegúrate de establecer las claves de API y configuraciones necesarias:
```
import getpass
import os

os.environ["LANGCHAIN_TRACING_V2"] = "true"
os.environ["LANGCHAIN_API_KEY"] = getpass.getpass("Ingresa tu clave de API de LangChain: ")
```

**4. Ejecutar el Notebook:**
Ejecuta el resto de las celdas en el notebook para ver el funcionamiento completo de RAG, incluyendo ejemplos de recuperación de información.

## Prueba

Respuesta final del laboratorio 👉 [📄](RespuestaFinal.txt)

![image](https://github.com/user-attachments/assets/bf4a6e4c-e642-40cc-b202-1b23ecaed234)


## Autor

- [Sebastián David Blanco Rodríguez](https://github.com/Sebastian2929)


## Licencia


Este proyecto está bajo la Licencia (MIT) - ver el archivo [LICENSE](LICENSE.md) para ver más detalles.
