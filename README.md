## 👋 Welcome to snipe-it 🚀

Open-source asset management system

## 📋 Description

Open-source asset management system

## 🚀 Services

- **snipe-it**: snipe/snipe-it:latest

### Infrastructure Components

- **snipe-it-db**: Mariadb database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/snipe-it/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/snipe-it" ~/.local/srv/docker/snipe-it
cd ~/.local/srv/docker/snipe-it
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install snipe-it
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:8072

## 📂 Volumes

- `./volumes/data/snipe-it` - Data storage
- `./volumes/config/snipe-it` - Data storage
- `./volumes/data/db/mariadb/snipe-it` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f snipe-it
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
