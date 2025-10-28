# OpenAEV Docker Deployment

Welcome to the OpenAEV Docker deployment guide! This guide provides resources and information to help you deploy and
manage OpenAEV using Docker.

---

## 📚 Documentation

For detailed instructions on installing OpenAEV using Docker, refer to
the [OpenAEV documentation space](https://docs.openaev.io/latest/deployment/installation/#using-docker).

---

## 👥 Community

### 🛠️ Status & Bugs

OpenAEV is actively under development. If you encounter bugs, have feature requests, or need help, please report them
using the [GitHub Issues module](https://github.com/OpenAEV-Platform/openaev/issues). We appreciate your feedback and
contributions to improve the platform.

### 💬 Discussions

Join our community to engage in discussions, share ideas, and get support:

- **Slack Channel:** Connect with us on [Slack](https://community.filigran.io)

---

## 🔧 Deployment Overview

### Quick Start with Docker Compose

The OpenAEV stack is modular and uses multiple Docker Compose files for easier configuration:

> [!IMPORTANT]
> Remember to create a .env file from .env.sample and customize the configuration as needed.

To start OpenAEV with the essential services, run:
```bash
   docker compose -p openaev -f docker-compose.yml up -d
```

To start OpenAEV with the Caldera executor (Caldera used as an agent), run:
```bash
   docker compose -p openaev -f docker-compose.yml -f docker-compose.caldera.yml -f docker-compose.caldera-executor.yml up -d
```

To start OpenAEV with the Caldera injector (Caldera used as an implant), run:
```bash
   docker compose -p openaev -f docker-compose.yml -f docker-compose.caldera.yml -f docker-compose.caldera-injector.yml up -d
```

#### Build Your Own Stack
OpenAEV allows you to customize your stack by selecting specific collectors and injectors to meet your unique needs:

- Additional Collectors: Explore a variety of collectors available [here](https://filigran.notion.site/OpenAEV-Ecosystem-30d8eb73d7d04611843e758ddef8941b#fb5f20e515df428994bed1438131cbd1).
- Additional Injectors: Discover injectors to enhance your simulations [here](https://filigran.notion.site/OpenAEV-Ecosystem-30d8eb73d7d04611843e758ddef8941b#90cfcc2895d441d68b54eda9b57d5d31).

## About

OpenAEV is a product designed and developed by the company [Filigran](https://filigran.io).

<a href="https://filigran.io" alt="Filigran"><img src="https://github.com/OpenAEV-Platform/openaev/raw/master/.github/img/logo_filigran.png" width="300" /></a>
