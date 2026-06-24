services:
  anisette:
    image: dadoum/anisette-v3-server
    expose:
      - "6969"

  web:
    image: nginx:alpine
    ports:
      - "80"
    volumes:
      - ./servers.json:/usr/share/nginx/html/servers.json:ro
      - ./nginx.conf:/etc/nginx/conf.d/default.conf:ro
