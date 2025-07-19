# ShortVideoByAI

> Dự án này tạo ra các video ngắn tự động bằng AI, kết hợp nhiều công nghệ hiện đại.

## Giới thiệu

ShortVideoByAI là một dự án sử dụng trí tuệ nhân tạo để tự động tạo ra các video ngắn. Dự án tận dụng các công nghệ mới như FastAPI cho backend, Google Text-to-Speech (TTS) để chuyển đổi văn bản thành giọng nói, và sử dụng các mô hình AI trên Replicate để tạo ảnh từ text.

## Công nghệ sử dụng

- **FastAPI**: Framework Python mạnh mẽ, được sử dụng để xây dựng backend với hiệu suất cao và dễ mở rộng.
- **Google TTS**: Tích hợp Google Text-to-Speech để chuyển đổi văn bản thành giọng nói tự nhiên.
- **Replicate**: Sử dụng các model AI trên nền tảng Replicate để sinh ảnh và tạo voice AI.
- **OpenAI**: Tích hợp các mô hình ngôn ngữ của OpenAI để sinh script (nội dung kịch bản) cho video.
- **Python**: Ngôn ngữ lập trình chính của dự án.

## Tính năng

- Tạo video ngắn tự động bằng AI.
- Chuyển đổi văn bản sang giọng nói bằng Google TTS.
- Sinh ảnh và voice bằng các model AI trên Replicate.
- Có thể mở rộng thêm các tính năng tuỳ ý.

## Cài đặt

1. Clone repository:
    ```bash
    git clone https://github.com/DatNewBie/ShortVideoByAI.git
    ```
2. Cài đặt các dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Sử dụng
- Chạy ứng dụng:

1. Frontend:
    ```bash
    npm run dev
    ```
2. Backend:
    ```bash
    py run.py
    ```
