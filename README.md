## Sample backends
```bash 
python3 -m http.server 2000
python3 -m http.server 3000
```

## NGINX
```
docker run --rm -it --name nginx -p4000:80 -v $(pwd):/etc/nginx/conf.d/:ro nginx
```

## HAProxy
```
docker run -it --rm --name haproxy -p4000:80 -v $(pwd):/usr/local/etc/haproxy/:ro --sysctl net.ipv4.ip_unprivileged_port_start=0 haproxy
```
