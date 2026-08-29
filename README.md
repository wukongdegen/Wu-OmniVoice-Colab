# Wu OmniVoice Studio — Google Colab

Chạy Wu OmniVoice Studio trên Google Colab bằng GPU, không cần cài đặt trên máy.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wukongdegen/Wu-OmniVoice-Colab/blob/main/Wu_OmniVoice_Colab.ipynb)

## Cách dùng

1. Bấm **Open In Colab**.
2. Chọn **Runtime → Change runtime type → T4 GPU** (hoặc L4/A100).
3. Bấm nút **Play ▶** ở ô `KHỞI CHẠY WU OMNIVOICE STUDIO`.
4. Cho phép kết nối Google Drive nếu muốn lưu kết quả lâu dài.
5. Chờ liên kết Gradio hoặc Cloudflare xuất hiện rồi mở Web UI.

Lần chạy đầu có thể mất vài phút để cài thư viện và tải model. Runtime Colab miễn phí có thể bị ngắt khi không hoạt động.

## Dữ liệu

Nếu bật lưu vào Google Drive, dữ liệu nằm trong `MyDrive/WuOmniVoice/`:

- `voice_store/` — giọng đã lưu và audio mẫu
- `Audio Output/` — audio đã tạo
- `Merged Videos/` — video đã ghép

## Bản phát hành

Notebook tự chọn gói binary Linux phù hợp với Python 3.12 hoặc 3.13 của runtime Colab từ GitHub Releases. Mã Python lõi được biên dịch bằng Cython để hạn chế đọc/sao chép trực tiếp; đây không phải cơ chế chống dịch ngược tuyệt đối.
