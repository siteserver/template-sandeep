# 模板介绍

模板名称：Sandeep

这是一套响应式网站模版，适应于企业、产品型公司以及各种企业集团网站模板所有图片在手机端都进行过处理，基于bootstrap响应式布局，兼容PC、平板、手机等主流媒体浏览。

### 模板文档

可以在模板文档 [https://sscms.com/docs/v7/official/advertisement/](https://sscms.com/docs/v7/official/advertisement/) 中查看模板的详细使用手册。

### 模板主页

可以访问模板主页 [https://sscms.com/templates/template.html?id=Sandeep](https://sscms.com/templates/template.html?id=Sandeep) 获取模板详细信息。


## 部署说明

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