events {}

http {
    server {
        listen 80;
        server_name _;

        location / {
            proxy_pass https://tonybnya-hng12-fastapi-book-project.onrender.com
            proxy_set_header Host $host;
            proxy_set_header X-Real-IP $remote_addr;
            proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
            proxy_ssl_verify off;
        }
    }
}
