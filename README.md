# Docker image for PocketBase

## Supported Architectures

Pulling `spectado/pocketbase:latest` will retrieve the correct image for your arch.

The architectures supported by this image are: **amd64**, **arm64** and **armv7**

## Application Setup

Access the webui at `<your-ip>:80`, for more information check out [PocketBase](https://pocketbase.io/docs/).

## Usage

**docker-compose**

```yml
version: "3.7"
services:
  pocketbase:
    image: ghcr.io/muchobien/pocketbase:latest
    container_name: pocketbase
    restart: unless-stopped
    ports:
      - "80:80"
    volumes:
      - /path/to/data:/pb_data
```

## Related Repositories

- [PocketBase](https://github.com/pocketbase/pocketbase)
