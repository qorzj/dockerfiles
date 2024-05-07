FROM node:20-slim
ENV PNPM_HOME="/pnpm"
ENV PATH="$PNPM_HOME:$PATH"
RUN apt-get update && apt-get install -y wget
RUN wget -qO- https://get.pnpm.io/install.sh | sh -
CMD ["pnpm", "version"]