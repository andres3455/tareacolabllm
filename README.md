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

configuramos las variables de entorno

```
import getpass
import os


os.environ["LANGSMITH_TRACING"] = "true"
os.environ["LANGSMITH_API_KEY"] = getpass.getpass()
```
ingresamos la api key de langsmith y utilizamos un modelo de lenguaje y ingreamos la Api key de OpenAi que nos suministro el profesor

```
pip install -qU "langchain[openai]"

import getpass
import os

if not os.environ.get("OPENAI_API_KEY"):
  os.environ["OPENAI_API_KEY"] = getpass.getpass("Enter API key for OpenAI: ")

from langchain.chat_models import init_chat_model

model = init_chat_model("gpt-4o-mini", model_provider="openai")
```
a partir de aqui podemos interactuar con el modelo

## Evidencias 

![image](https://github.com/user-attachments/assets/38fd3ca5-73ff-4ede-8001-ec164fe76964)



