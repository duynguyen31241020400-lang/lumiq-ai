# Lumiq AI

**Công cụ học tập cá nhân hóa – Rèn luyện tư duy tự học.**

Lumiq AI không chỉ là một nền tảng hỗ trợ học tập, mà là **công cụ giúp học sinh xây dựng năng lực tự học**. 

Chúng tôi tập trung vào việc **cá nhân hóa hành trình học tập** và **rèn luyện tư duy tự chủ** – giúp người học không chỉ biết mình yếu ở đâu, mà còn biết cách tự xác định mục tiêu, tự điều chỉnh phương pháp và tự theo dõi tiến độ của chính mình.

## 🎯 Định hướng sản phẩm

- **Cá nhân hóa thực sự**: Mỗi học sinh có một lộ trình học tập riêng, xuất phát từ điểm yếu thực tế thay vì chương trình chung chung.
- **Rèn luyện tư duy tự học**: AI Tutor không chỉ giải bài, mà hướng dẫn học sinh cách suy nghĩ, đặt câu hỏi và tự khám phá kiến thức.
- **Xây dựng thói quen học tập bền vững**: Tập trung vào việc hình thành năng lực tự giác và kỹ năng tự điều chỉnh thay vì chỉ chạy theo điểm số.

## ✨ Tính năng cốt lõi

- **Đánh giá chẩn đoán nhanh**: 6 câu hỏi giúp xác định chính xác năng lực hiện tại ở các chủ đề trọng tâm.
- **Mục tiêu học tập cá nhân hóa (Current Goal)**: Sau mỗi lần đánh giá, hệ thống tự động đề xuất mục tiêu ngắn hạn rõ ràng, phù hợp với năng lực và nhu cầu của từng người học.
- **AI Tutor đồng hành phát triển tư duy**: Tutor phản hồi theo ngữ cảnh học tập thực tế, khuyến khích học sinh tư duy độc lập thay vì chỉ cung cấp đáp án.
- **Theo dõi và điều chỉnh liên tục**: Học sinh có thể nhìn thấy sự tiến bộ và tự điều chỉnh hướng đi học tập của mình.

## 🛠️ Công nghệ

- Next.js 15 (App Router) + TypeScript + Tailwind CSS
- Google Gemini + RAG (Hybrid Search)
- Supabase (PostgreSQL + Vector)
- Vercel

## 🚀 Chạy locally

### Yêu cầu

- Node.js 18 trở lên
- Supabase project
- Google Gemini API Key

### Cài đặt

\\\ash
git clone https://github.com/duynguyen31241020400-lang/lumiq-ai.git
cd lumiq-ai
npm install
cp .env.example .env.local
\\\

### Biến môi trường

Tạo file \.env.local\:

\\\env
GEMINI_API_KEY=your_gemini_api_key

NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
\\\

### Khởi chạy

\\\ash
npm run dev
\\\

Truy cập [http://localhost:3000](http://localhost:3000)

## 📁 Cấu trúc thư mục chính

\\\
src/
├── app/
│   ├── assessment/          # Đánh giá đầu vào
│   ├── learn/math/          # Lộ trình cá nhân hóa + AI Tutor
│   └── api/chat/
├── components/learning/     # ProgressTree, TutorChat
└── lib/
    ├── ai/                  # Prompt Engine + RAG logic
    └── data/                # Dữ liệu năng lực & câu hỏi
\\\

## 📌 Phạm vi hiện tại (Phase 1)

Phiên bản demo hiện tại được thiết kế dành riêng cho **học sinh lớp 10, môn Toán**.  
Chi tiết về giai đoạn này được mô tả tại file [README_IU_Startup_Demo_Day.md](./README_IU_Startup_Demo_Day.md).

## 📄 License

MIT License
