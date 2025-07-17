FROM node:20-bullseye
ENV PNPM_HOME="/pnpm"
ENV PATH="$PNPM_HOME:$PATH"
ENV HTTPS_PROXY="http://192.168.65.19:1087"
RUN curl -fsSL https://get.pnpm.io/install.sh | ENV="$HOME/.bashrc" SHELL="$(which bash)" bash -
RUN pnpm install -g vercel
CMD ["pnpm", "version"]
