FROM python:3.11-slim

# Tạo thư mục làm việc trong container
WORKDIR /app

# Copy file requirements.txt trước (tối ưu cache layer)
COPY backend/requirements.txt .

# Cài đặt thư viện Python
RUN pip install --no-cache-dir -r requirements.txt

# Copy toàn bộ mã nguồn backend vào container
COPY backend/ .

# Expose port nếu bạn có chạy server (ví dụ Flask/FastAPI), nếu không thì có thể bỏ
EXPOSE 8000

# Lệnh chạy app
CMD ["python", "run.py"]
