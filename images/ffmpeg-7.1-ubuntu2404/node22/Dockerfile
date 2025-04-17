# 基于jrottenberg/ffmpeg镜像  
FROM jrottenberg/ffmpeg:7.1-ubuntu2404  

# 安装Node.js  
RUN apt-get update && apt-get install -y curl && \
    curl -fsSL https://deb.nodesource.com/setup_22.x | bash - && \
    apt-get install -y nodejs && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/*  

# 验证安装  
RUN node --version && npm --version && ffmpeg -version  

# 设置工作目录  
WORKDIR /app  

# 默认命令  
ENTRYPOINT []
CMD [ "node" ]