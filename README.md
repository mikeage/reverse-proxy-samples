```bash
# Servers
python3 -m http.server 2000
python3 -m http.server 3000

# Reverse proxy
docker run --rm -it --name nginx -p4000:80 -v $(pwd):/etc/nginx/conf.d/:ro nginx
```
