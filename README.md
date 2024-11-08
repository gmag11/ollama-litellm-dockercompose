# [ollama-litellm-dockercompose - GitHub]()

# **Español**

## ollama-litellm-dockercompose

Este repositorio proporciona archivos de configuración y un archivo `docker-compose.yaml` para facilitar la ejecución de Open WebUI y LiteLLM con un esfuerzo mínimo.

### Contenido del repositorio

- `.env`: Archivo de variables de entorno donde deben añadirse las claves API de los proveedores de modelos (como OpenAI, Anthropic, OpenRouter, etc.).
- `docker-compose.yaml`: Archivo de configuración de Docker Compose.
- `litellm_config.yaml`: Archivo de configuración para LiteLLM, donde se pueden añadir y configurar modelos adicionales según las necesidades.

### Requisitos previos

- Docker

### Instrucciones de uso

1. **Clonar el repositorio:**

   ```bash
   git clone https://github.com/gmag11/ollama-litellm-dockercompose.git
   cd ollama-litellm-dockercompose
   ```

2. **Configurar las variables de entorno:**

   Edite el archivo `.env` para añadir las claves API de los proveedores de modelos necesarios (como OpenAI, Anthropic, OpenRouter, entre otros) según los modelos que planee utilizar.

3. **Configurar modelos adicionales (opcional):**

   Puede añadir más modelos en el archivo `litellm_config.yaml`, siguiendo las instrucciones de configuración disponibles en [la documentación de LiteLLM](https://docs.litellm.ai/docs/providers). Esto permite personalizar y ampliar los modelos que estarán disponibles en LiteLLM.

4. **Iniciar los servicios:**

   ```bash
   docker-compose up -d
   ```

   Esto iniciará los servicios en segundo plano.

5. **Acceder a Open WebUI:**

   Abra su navegador web y navegue a `http://localhost:3000` para acceder a Open WebUI.

### Notas adicionales

- Asegúrese de que los puertos especificados en el archivo `docker-compose.yaml` no estén en uso por otros servicios en su sistema.
- Para detener los servicios, ejecute:

  ```bash
  docker-compose down
  ```

# **English**

## ollama-litellm-dockercompose

This repository provides configuration files and a `docker-compose.yaml` file to facilitate running Open WebUI and LiteLLM with minimal effort.

### Repository Contents

- `.env`: Environment variables file where API keys for model providers (such as OpenAI, Anthropic, OpenRouter, etc.) should be added.
- `docker-compose.yaml`: Docker Compose configuration file.
- `litellm_config.yaml`: Configuration file for LiteLLM, where additional models can be added and configured as needed.

### Prerequisites

- Docker

### Usage Instructions

1. **Clone the repository:**

   ```bash
   git clone https://github.com/gmag11/ollama-litellm-dockercompose.git
   cd ollama-litellm-dockercompose
   ```

2. **Configure environment variables:**

   Edit the `.env` file to add the necessary API keys for the model providers you plan to use (such as OpenAI, Anthropic, OpenRouter, among others).

3. **Configure additional models (optional):**

   You can add more models in the `litellm_config.yaml` file, following the configuration instructions available in [LiteLLM documentation](https://docs.litellm.ai/docs/providers). This allows customization and expansion of models available in LiteLLM.

4. **Start the services:**

   ```bash
   docker-compose up -d
   ```

   This will start the services in the background.

5. **Access Open WebUI:**

   Open your web browser and navigate to `http://localhost:8080` to access Open WebUI.

### Additional Notes

- Ensure that the ports specified in the `docker-compose.yaml` file are not in use by other services on your system.
- To stop the services, run:

  ```bash
  docker-compose down
  ```
