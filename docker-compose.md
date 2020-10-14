# Docker Compose Snippets


## PostgreSQL

```yaml
version: "3"

volumes:
  my-volume: {}
  
services:
  pg:
    image: postgres:13.0
    environment:
      POSTGRES_USER: admin
      POSTGRES_PASSWORD: secret
      POSTGRES_DB: data
    ports:
      - "5432:5432"
    volumes:
      - "my-volume:/var/lib/postgresql/data"
```
