FROM node:20-bookworm

# 1. install pnpm & utilities
RUN corepack enable && pnpm setup

# 2. supabase cli for local stack + migrations
RUN npm i -g supabase@latest

# 3. clean dev tooling
WORKDIR /workspace
