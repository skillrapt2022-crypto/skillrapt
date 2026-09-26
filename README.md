# SKILLRAPT Corporate Website & Administrative Platform

> **"INDUSTRY - ACADEMIA - CONNECT"**  
> Official corporate website and course administration system for **SkillRapt India Private Limited**.

---

## 🌟 Overview

SkillRapt is a premier engineering training, skill development, internship, placement assistance, and campus training organization focused on bridging the gap between academic education and industry requirements.

This repository contains the complete, production-ready, full-stack website built with **Next.js 14 (App Router)**, **TypeScript**, **Tailwind CSS**, **Prisma ORM**, and **PostgreSQL/SQLite**.

---

## 🏢 Business Locations

### 1. CHENNAI HEAD OFFICE
**SkillRapt India Private Limited**  
No.27, Customs Colony,  
1st Main Road, Thoraipakkam,  
OMR, Chennai - 600097,  
Tamil Nadu, India.

### 2. POLLACHI BRANCH
**SkillRapt**  
5/4 V K R Street,  
Venkatesa Colony,  
Near Sakthi Hotel,  
Pollachi - 642001,  
Coimbatore District,  
Tamil Nadu, India.

---

## 📞 Official Contact Details
- **Phones**: +91 79044 43878 / +91 91761 31866
- **Email**: info@skillrapt.in
- **Website**: www.skillrapt.in
- **WhatsApp**: +91 79044 43878

---

## 🛠️ Technology Stack

- **Framework**: Next.js 14+ (App Router, TypeScript)
- **Styling**: Tailwind CSS with custom SkillRapt Deep Navy (`#0B1B3D`) & SkillRapt Orange (`#FF6B00`) theme
- **Icons**: Lucide React
- **ORM & Database**: Prisma ORM with SQLite (Local Dev) / PostgreSQL (Production)
- **Authentication**: JWT token authentication stored in HTTP-only secure cookies
- **Validation**: Zod schema validation
- **SEO**: Dynamic JSON-LD structured data (EducationalOrganization / LocalBusiness), Metadata API, dynamic `sitemap.ts`, `robots.ts`

---

## 🚀 Getting Started

### 1. Installation
```bash
npm install
```

### 2. Database Sync & Seeding
Sync Prisma schema and seed initial database (Super Admin user, official branches, 7 engineering departments, 10 core services, 18+ courses, FAQs):
```bash
npx prisma db push
node prisma/seed.js
```

### 3. Start Local Development Server
```bash
npm run dev
```
Open [http://localhost:3000](http://localhost:3000) in your browser.

---

## 🔐 Admin Dashboard Access

- **Route**: `/admin/login` or `/admin`
- **Default Super Admin Email**: `admin@skillrapt.in`
- **Default Super Admin Password**: `SkillRapt@2026!`

### Admin Capabilities:
1. **Dashboard Overview**: Track metrics (Total/Active Courses, Total/New Enquiries, Branch breakdown).
2. **Course CRUD**: Create new course, update curriculum & technologies, toggle active status, or delete course.
3. **Enquiry Management**: Filter leads by status (`NEW`, `CONTACTED`, `IN_PROGRESS`, `CONVERTED`, `CLOSED`) and branch (`CHENNAI`, `POLLACHI`, `ONLINE`), update status, and record internal staff notes.

---

## 📦 Production Build & Deployment

To generate an optimized production build:
```bash
npm run build
npm run start
```

### Vercel / Railway / Render Deployment
1. Set Environment Variables:
   - `DATABASE_URL`: PostgreSQL connection string (Supabase / Neon / Railway)
   - `JWT_SECRET`: Secure secret string
   - `NEXT_PUBLIC_SITE_URL`: `https://www.skillrapt.in`
   - `NEXT_PUBLIC_WHATSAPP_NUMBER`: `917904443878`
2. Deploy to Vercel with zero extra build configuration required.

---

## 📄 Copyright & Licensing
© 2026 SkillRapt India Private Limited. All Rights Reserved.

## Latest SkillRapt updates

This version includes:
- Fixed hero engineering carousel sizing with local image fallbacks.
- Exact department order on the homepage and Courses page: Mechanical, Civil, EEE, ECE, Mechatronics, CSE / IT, AI & Data Science / ML / Robotics.
- Courses page fallback to the local course catalog when the database/API has no public course records.
- CSE / IT and EEE course poster gallery using the supplied SkillRapt brochure assets.
- Placement Success Stories gallery using the supplied testimonial assets.
- SkillRapt YouTube channel CTA in the Services Ecosystem section.
- A working `/services` page for the Services Ecosystem links.
- More consistent training-area card alignment.

For Windows setup, see `RUN-WINDOWS.txt`.
