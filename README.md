# OpenWebUI + Ollama (Docker)

Stack locale pour faire tourner des modèles de langage (LLM) en local avec [Ollama](https://ollama.com) pour l'inférence et [OpenWebUI](https://github.com/open-webui/open-webui) comme interface web de chat.

## Installation

1. Cloner le repo :

   ```bash
   git clone <https://github.com/JeremyLrs/open-webui.git>
   ```

2. Lancer les containers :

   ```bash
   docker compose up -d
   ```

## Télécharger un modèle

Les modèles ne sont pas inclus dans le repo. Après le premier lancement, il faut en télécharger au moins un :

```bash
docker exec -it ollama ollama pull llama3.2
```

D'autres modèles utiles selon le besoin :

`qwen3:8b` `qwen3-coder` `ministral-3:8b`    
```

## Accéder à l'interface

Une fois les containers démarrés, ouvrir :

```
http://localhost:3000
```

La première connexion demande de créer un compte administrateur.
