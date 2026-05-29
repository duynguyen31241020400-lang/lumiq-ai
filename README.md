# Lumiq AI

**Học Toán lớp 10 đúng chỗ, đúng lúc.**

Lumiq AI là công cụ hỗ trợ học tập cá nhân hóa dành cho học sinh lớp 10, giúp các em nhanh chóng xác định điểm yếu môn Toán và nhận lộ trình học tập tập trung cùng AI Tutor thông minh.

## ✨ Tính năng nổi bật

- **Đánh giá nhanh (6 câu)**: Chỉ cần 6 câu hỏi để chẩn đoán chính xác năng lực ở 3 chủ đề Toán lớp 10 quan trọng (Tập hợp, Phép toán tập hợp, Hàm bậc hai).
- **Current Goal rõ ràng**: Sau khi làm bài, hệ thống tự động xác định chủ đề yếu nhất và đặt ra mục tiêu học tập ngắn hạn cụ thể.
- **AI Tutor theo ngữ cảnh**: Tutor không trả lời chung chung mà luôn bám sát:
  - Chủ đề đang học
  - Điểm yếu hiện tại của học sinh
  - Mục tiêu ngắn hạn
- **Trải nghiệm mượt mà**: Giao diện hiện đại, tối ưu cho thiết bị di động, hỗ trợ PWA.

## 🛠️ Công nghệ sử dụng

- **Frontend**: Next.js 15 (App Router), TypeScript, Tailwind CSS
- **AI**: Google Gemini API + Hybrid Search (RAG)
- **Database**: Supabase (PostgreSQL + pgvector)
- **Triển khai**: Vercel

## 🚀 Chạy locally

### Yêu cầu

- Node.js 18+
- Tài khoản Supabase
- Google Gemini API Key

### Cài đặt

\\\ash
# Clone repository
git clone https://github.com/duynguyen31241020400-lang/lumiq-ai.git
cd lumiq-ai

# Cài đặt dependencies
npm install

# Tạo file .env.local và điền thông tin
cp .env.example .env.local
\\\

### Biến môi trường cần thiết

Tạo file \.env.local\ với các biến sau:

\\\env
# Google Gemini
GEMINI_API_KEY=your_gemini_api_key

# Supabase
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
\\\

### Chạy ứng dụng

\\\ash
npm run dev
\\\

Mở [http://localhost:3000](http://localhost:3000) để xem kết quả.

## 📁 Cấu trúc thư mục

\\\
src/
├── app/                  # Next.js App Router
│   ├── assessment/       # Bài đánh giá đầu vào
│   ├── learn/math/       # Lộ trình học + AI Tutor
│   └── api/chat/         # API cho AI Tutor
├── components/
│   ├── learning/         # ProgressTree, TutorChat
│   └── ui/               # Các component chung
└── lib/
    ├── ai/               # Logic RAG + Gemini (prompt engine)
    ├── data/             # Dữ liệu năng lực & câu hỏi
    └── demo-state.ts     # Quản lý kết quả assessment
\\\

## 📝 Lưu ý

- Ứng dụng hiện đang tập trung vào **Toán lớp 10** (3 chủ đề: M10.1, M10.2, M10.3).
- AI Tutor sử dụng kỹ thuật **RAG** kết hợp kiến thức dự phòng để đảm bảo trải nghiệm ổn định.
- Dữ liệu học sinh được lưu tạm thời trên trình duyệt (localStorage) trong phiên demo.

## 📄 License

MIT License

---

**Lumiq AI** — Học đúng chỗ, tiến bộ rõ rệt.
