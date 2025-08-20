# Stage 1: Build Vite app
FROM node:18 AS builder

WORKDIR /app

# Copy package files và cài dependencies
COPY frontend/package*.json ./
RUN npm install

# Copy toàn bộ mã nguồn
COPY frontend/ ./

# Build Vite app (output sẽ ở thư mục /app/dist)
RUN npm run build

# Stage 2: Serve bằng nginx
FROM nginx:alpine

# Copy file từ dist → nginx html
COPY --from=builder /app/dist /usr/share/nginx/html
COPY frontend/nginx.conf /etc/nginx/conf.d/default.conf

# Expose port 80
EXPOSE 80

# Start nginx
CMD ["nginx", "-g", "daemon off;"]
