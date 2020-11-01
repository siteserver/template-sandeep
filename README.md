# 部署说明

``` bash
docker run -d \
    --name sandeep \
    -p 80:80 \
    --restart=always \
    -v "$(pwd)"/wwwroot:/app/wwwroot \
    -e SSCMS_SECURITY_KEY=e2a3d303-ac9b-41ff-9154-930710af0845 \
    -e SSCMS_DATABASE_TYPE=SQLite \
    sscms/core:latest
```