FROM node:20-bookworm

# 1. install pnpm & utilities
RUN corepack enable && corepack prepare pnpm@latest --activate

# 2. supabase cli for local stack + migrations
ARG SUPABASE_VERSION=2.30.4 # ⬅︎ check “latest” before building 
RUN curl -fsSL https://github.com/supabase/cli/releases/download/v${SUPABASE_VERSION}/supabase_${SUPABASE_VERSION}_linux_amd64.tar.gz 

# 3. clean dev tooling
WORKDIR /workspace
