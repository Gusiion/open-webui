### Download container
```bash
docker pull ghcr.io/sunkendreams/voltron-webui:ollama
```

### Run Voltron container
```bash
docker run -d -p 3300:8080 --gpus=all -v voltron:/root/.ollama -v voltron-webui:/app/backend/data --name voltron --restart always ghcr.io/sunkendreams/voltron-webui:ollama
```
