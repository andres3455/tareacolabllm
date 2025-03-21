# Creando una aplicación de LLM sencilla con modelos de chat y plantillas de sugerencias

### Dessarollado por: 
* Andrés Felipe Rodríguez Chaparro

## Arquitectura y Componentes
La aplicación se compone de los siguientes componentes principales:

Modelos de Lenguaje (LLM): Se utiliza un modelo de lenguaje grande (LLM) proporcionado por OpenAI para generar las traducciones.​
OpenWebinars.net

Plantillas de Prompt: Se define una plantilla de prompt que especifica cómo se debe solicitar la traducción al LLM.​
Introduction | 🦜️🔗 LangChain

LLMChain: Es una cadena que combina el LLM y la plantilla de prompt para procesar las solicitudes de traducción.​

La arquitectura de LangChain permite combinar estos componentes de manera modular, facilitando la construcción y escalabilidad de aplicaciones basadas en LLM.

## Instalación

Instalamos las dependencias necesarias

```
pip install langchain
```

debemos ingresar y crear una cuenta en langsmith, al hacer eso, creamos un nuevo proyecto y nos generara una api key

```
https://smith.langchain.com/o/92d0b5f1-fc75-49c1-b2a9-45d14ce7a89a
```




