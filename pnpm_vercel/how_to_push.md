docker-compose build
docker login --username="goodhorsezxj@gmail.com" registry.cn-hangzhou.aliyuncs.com
# 输入密码，安全起见每次在阿里云「容器镜像服务/实例列表/访问凭证」页面设置固定密码，使用之后修改为不知道的新密码
docker tag qorzj/pnpm_vercel:latest registry.cn-hangzhou.aliyuncs.com/qorzj/pnpm_vercel:latest
docker push registry.cn-hangzhou.aliyuncs.com/qorzj/pnpm_vercel:latest
