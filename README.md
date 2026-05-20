# Master Workflow — หน่วยทวนสอบก๊าซเรือนกระจก (VB)

> Interactive workflow diagram for a Greenhouse Gas Verification Body (VB) operating under **ISO 14065:2020** + **ISO/IEC 17029**, covering the full lifecycle from organization setup to continuous improvement.

🌐 **Live Demo:** *[เพิ่ม URL หลังเปิด GitHub Pages]*

---

## 📋 ภาพรวม (Overview)

เอกสาร HTML แบบ self-contained ที่แสดง **swim-lane workflow diagram** ครบทั้ง 10 phase ของหน่วยทวนสอบก๊าซเรือนกระจก (Verification Body — VB) ตามมาตรฐาน ISO 14065 และ ISO/IEC 17029 พร้อมระบบ **click-to-detail** ที่คลิกได้แต่ละกล่องเพื่อดูรายละเอียดของกิจกรรม

This is a self-contained HTML document that visualizes the complete workflow of a Greenhouse Gas Verification Body in 10 phases — from initial setup through PDCA continuous improvement — with interactive click-to-reveal details on every activity.

---

## ✨ Features

- 📊 **10 Swim-Lane Diagrams** — ครบทุก phase ตั้งแต่จัดตั้งหน่วย → ปรับปรุงระบบ
- 🖱️ **Interactive Click-to-Detail** — คลิกที่กล่องใดก็ได้ในแผน เพื่อดู
  - ⏰ ความถี่ที่ต้องทำ (Frequency)
  - 👤 ผู้รับผิดชอบ (Responsible person)
  - 📄 เอกสารที่ใช้ (Documents — FM/RE/WI/PM/QM)
  - 📋 ขั้นตอนละเอียด (Step-by-step procedure)
  - 🎯 Output / สิ่งที่ต้องส่งมอบ (Deliverable)
  - 💡 ข้อควรระวัง (Notes & warnings)
  - 🔗 เอกสารที่เกี่ยวข้อง (Related documents)
- 🎨 **Color-coded by Role** — MD / QMR / HR / Auditor / Client / JR / Committee / Accounting
- 📱 **Responsive** — เปิดได้บน Desktop, iPad, มือถือ
- 🖨️ **Print-Friendly** — กด `Ctrl+P` / `Cmd+P` เพื่อพิมพ์เป็น PDF
- 🇹🇭 **Thai language** — ภาษาไทย พร้อมศัพท์เทคนิคภาษาอังกฤษ

---

## 📑 10 Phases ที่ครอบคลุม

| # | Phase | ครอบคลุม |
|---|---|---|
| **NO.01** | การจัดตั้งหน่วยทวนสอบ (Foundation) | QM-01 + ทุก PM/RE/WI + ขอรับรอง สมอ. |
| **NO.02** | คณะกรรมการเพื่อความเป็นกลาง (Committee) | PM-13 + RE-03 (6 ภาคส่วน) |
| **NO.03** | การสรรหาบุคลากร (HR Recruitment) | PM-06 + PM-08 |
| **NO.04** | คัดเลือก/แต่งตั้งผู้ทวนสอบ (Auditor Selection) | PM-07 + RE-02 + WI-01 + WI-03 |
| **NO.05** | วางระบบความเสี่ยง/ความเป็นกลาง (Planning) | PM-10 + PM-15 + PM-17 |
| **NO.06** | รับบริการทวนสอบ (Intake) | PM-09 + WI-04 + WI-05 |
| **NO.07** | ดำเนินการทวนสอบหน้างาน (Verification) | PM-12 + WI-02 + WI-03 |
| **NO.08** | ทบทวน-ตัดสิน-ออกถ้อยแถลง (Statement) | PM-12 + PM-16 + RE-01 |
| **NO.09** | การจัดการร้องเรียน/อุทธรณ์ (Complaint) | PM-11 |
| **NO.10** | การปรับปรุงระบบ PDCA (Improvement) | PM-02 + PM-04 + PM-05 + PM-15 |

ครอบคลุม **53 กิจกรรม** ที่มีคำอธิบายละเอียดเปิดผ่านระบบ modal popup

---

## 🚀 วิธีใช้งาน

### 1. ใช้ Local

ดาวน์โหลดไฟล์ `index.html` แล้วเปิดด้วย Web Browser (Chrome, Safari, Edge, Firefox)

### 2. Publish on GitHub Pages

```bash
# 1) สร้าง repository ใหม่บน GitHub
git init
git add .
git commit -m "Initial commit: Master Workflow"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main

# 2) เปิด GitHub Pages
# Settings → Pages → Source: Deploy from a branch → main → / (root)
```

หลังจาก GitHub Pages เปิดใช้งานแล้ว ไฟล์ `index.html` จะเข้าถึงได้ที่:
```
https://<your-username>.github.io/<repo-name>/
```

### 3. Embed / Iframe

```html
<iframe src="https://<your-username>.github.io/<repo-name>/"
        width="100%" height="900" frameborder="0">
</iframe>
```

---

## ⌨️ Keyboard Shortcuts

| Key | Action |
|---|---|
| **Click** กล่อง / กรอบ diamond | เปิด modal แสดงรายละเอียด |
| **Esc** | ปิด modal |
| **Ctrl+P** / **Cmd+P** | พิมพ์เป็น PDF |

---

## 🛠️ Technical Details

- **Pure HTML/CSS/JavaScript** — ไม่ต้องลง dependency ใดๆ
- **SVG-based diagrams** — คมชัด ไม่แตก zoom ได้
- **Self-contained** — ไฟล์เดียวจบ ไม่ต้องโหลด assets เพิ่ม
- **Browser support** — Chrome, Safari, Firefox, Edge (เวอร์ชั่นใหม่)
- **Font fallback** — `Sarabun`, `TH Sarabun New`, `Noto Sans Thai`, system-ui

---

## 📂 Document System Reference

The workflow references these documents:

- **QM-01** — Quality Manual
- **PM-01 to PM-17** — Procedure Manuals (16 docs, no PM-14)
- **RE-01 to RE-03** — Regulations
- **WI-01 to WI-05** — Work Instructions
- **FM-01 to FM-72** — Forms

---

## 🏢 About

Created for **Verification Body (VB) operating under ISO 14065** for CFO (Carbon Footprint for Organization) verification, accredited by **TGO Thailand** (Thailand Greenhouse Gas Management Organization).

---

## 📜 License

This workflow template is provided for educational reference. The procedures and document codes referenced (PM/RE/WI/FM) are aligned with ISO 14065:2020 and ISO/IEC 17029 requirements.

---

## 🤝 Contributing

Found an error in a workflow step or want to suggest improvements?

1. Open an [Issue](../../issues) with the activity code (e.g., `a35`)
2. Submit a Pull Request with edits to the relevant section

---

## 📞 Contact

For inquiries about implementation in your organization, please reach out via the repository Issues page.
