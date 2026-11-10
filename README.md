<p align="center">
    <a href="https://fryrvo.com" target="_blank" rel="noopener noreferrer">
        <img src="https://cdn.fryrvo.com/assets/fryrvo_branding/Logo_bg.png" alt="icon" width="120">
    </a>
</p>

<div align="center">

# Git Mirror
Source code for the Fryrvo git mirror.

</div>

> [!NOTE]
> **Note:** This repository is a fork of [gitea-mirror](https://github.com/RayLabsHQ/gitea-mirror). 

---

## Deployment

1. **Clone the repository**
```bash
git clone https://git.lgbt/fryrvo/git-mirror.git && cd git-mirror
```


2. **Start with Docker Compose**
```bash
docker compose -f docker-compose.alt.yml up -d
```

3. **Update**
```bash
git pull && docker compose -f docker-compose.alt.yml pull && docker compose -f docker-compose.alt.yml up -d
```

---

## Contributing
If you want to run or modify the project locally

1. **Install**
```bash
bun install
```

2. **Start the server**
```bash
bun run dev
```

3. **Build**
```bash
docker build -t ghcr.io/fryrvo/git-mirror:latest .
docker push ghcr.io/fryrvo/git-mirror:latest
```