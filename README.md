# 🏘️ Community Platform — Graduation Project

เว็บไซต์ชุมชนออนไลน์ครบวงจร ที่ช่วยกระจายข่าวสาร จัดกิจกรรม และเชื่อมต่อผู้คนในชุมชนเดียวกัน
สร้างขึ้นเพื่อแก้ปัญหาการสื่อสารที่กระจัดกระจายภายในชุมชน โดยรวมฟีเจอร์ Blog, Event, Social Interaction และ Real-time Chat ไว้ในที่เดียว

> 🎓 โปรเจกต์จบการศึกษา — พัฒนาโดย [Natthaphan Latea](https://github.com/XAN44)

<!-- 🔗 ใส่ลิงก์ live demo ตรงนี้ถ้ามี -->
<!-- ## 🎬 Live Demo -->
<!-- [ดู Demo ที่นี่](#) -->

<!-- 📸 แนะนำให้แนบ screenshot หรือ GIF การใช้งานตรงนี้ จะช่วยให้คนอ่านเห็นภาพเร็วขึ้นมาก -->

---

## ✨ Features

**Content**
- 📰 **Blog** — เขียนบทความด้วย Rich Text Editor (Tiptap/Quill)
- 📅 **Event** — สร้างและจัดการกิจกรรม/การนัดหมายในชุมชน
- 📝 **Post** — แชร์เนื้อหาชีวิตประจำวัน

**Social**
- 💬 **Real-time Chat** ด้วย Socket.io + Pusher
- 👍 **Like / Follow** — ติดตามและมีส่วนร่วมกับเนื้อหา
- 👤 **User Profile** — จัดการโปรไฟล์ส่วนตัว

**Auth & Upload**
- 🔐 **Google OAuth** ผ่าน NextAuth
- 🖼️ **อัปโหลดรูปภาพ** ผ่าน Cloudinary / EdgeStore / Uploadthing

---

## 🏗️ Tech Stack

| Category  | Technology |
| --------- | ---------- |
| Framework | Next.js 14, TypeScript |
| Real-time | Socket.io + Pusher (custom server) |
| Auth      | NextAuth (Auth.js) + Google OAuth |
| ORM       | Prisma |
| Database  | PostgreSQL / MySQL / Supabase |
| State     | Zustand + SWR |
| UI        | TailwindCSS, Radix UI, NextUI, Mantine, Chakra UI |
| Form      | React Hook Form + Zod |
| Editor    | Tiptap + Quill |
| Dev Watch | Nodemon |

---

## 📁 โครงสร้างโปรเจกต์

```
├── server/          # Custom server — Socket.io + Express
├── prisma/          # Database schema
├── drawing.drawio   # Database design diagram
├── rest.http        # API testing
├── src/             # Next.js app directory
└── nodemon.json     # Watch server
```

---

## 🚀 เริ่มใช้งาน

```bash
git clone https://github.com/XAN44/social-media-platform.git
cd social-media-platform
npm install

# ตั้งค่า environment variables ของคุณเอง (ดู .env.example)
cp .env.example .env

npx prisma db push
npm run dev
```

**Environment variables ที่ต้องตั้งค่า:**
```
DATABASE_URL=
NEXTAUTH_SECRET=
GOOGLE_CLIENT_ID=
GOOGLE_CLIENT_SECRET=
```

> ⚠️ โปรเจกต์นี้ต้องรันผ่าน custom server (`server/`) เสมอ เนื่องจากใช้ Socket.io — **ไม่รองรับการ deploy บน Vercel** แนะนำ Railway, Render หรือ VPS แทน

---

## 📌 หมายเหตุ

โปรเจกต์นี้พัฒนาเพื่อวัตถุประสงค์ทางการศึกษา (Graduation Project) เน้นฝึกฝนการออกแบบสถาปัตยกรรมระบบแบบ full-stack ที่มี Real-time feature และ Authentication ที่ปลอดภัย

---

## 📬 Contact

Natthaphan Latea — [nattapanlateh26@gmail.com](mailto:nattapanlateh26@gmail.com) · [GitHub](https://github.com/XAN44)
