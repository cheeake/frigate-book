
---
hide:
  - navigation
---

# คู่มือ Frigate NVR ฉบับสมบูรณ์

!!! tip "จากศูนย์สู่ระบบกล้องวงจรปิด AI ที่ใช้งานได้จริง"
    คู่มือภาษาไทยครบทุกขั้นตอน ตั้งแต่เลือกฮาร์ดแวร์ ติดตั้ง จูนค่า
    ไปจนถึงเชื่อมต่อ Home Assistant และแก้ปัญหาที่เจอบ่อย

[เริ่มอ่านบทที่ 1 :material-arrow-right:](01-intro.md){ .md-button .md-button--primary }
[ดู Config พร้อมใช้](appendix-a.md){ .md-button }

---

## เนื้อหาในเล่ม

<div class="grid cards" markdown>

-   :material-book-open-variant:{ .lg .middle } **ภาค 1 — พื้นฐาน**

    ---

    ทำความเข้าใจว่า Frigate คืออะไร ทำงานอย่างไร
    และทำไม Dual-Stream ถึงสำคัญ

    [:octicons-arrow-right-24: เริ่มอ่าน](01-intro.md)

-   :material-chip:{ .lg .middle } **ภาค 2 — เตรียมความพร้อม**

    ---

    เลือก CPU/GPU/Coral เลือกกล้อง
    และคำนวณพื้นที่จัดเก็บให้พอใช้

    [:octicons-arrow-right-24: เลือกฮาร์ดแวร์](04-hardware.md)

-   :material-docker:{ .lg .middle } **ภาค 3 — ติดตั้ง**

    ---

    Docker Compose, Home Assistant Add-on,
    Proxmox LXC และ go2rtc

    [:octicons-arrow-right-24: ติดตั้ง](07-docker.md)

-   :material-file-cog:{ .lg .middle } **ภาค 4 — Config**

    ---

    เจาะลึก config.yml ทุกส่วน
    Detectors, Zones, Recording, Snapshots

    [:octicons-arrow-right-24: ดู Config](10-config-structure.md)

-   :material-tune:{ .lg .middle } **ภาค 5 — จูนให้เทพ**

    ---

    ลด False Positive จูนประสิทธิภาพ
    และใช้ Semantic Search / Face / LPR

    [:octicons-arrow-right-24: จูนระบบ](16-false-positive.md)

-   :material-home-assistant:{ .lg .middle } **ภาค 6 — เชื่อมต่อ**

    ---

    Home Assistant, MQTT
    และสร้าง Automation แจ้งเตือน

    [:octicons-arrow-right-24: เชื่อมต่อ](20-homeassistant.md)

-   :material-wrench:{ .lg .middle } **ภาค 7 — ดูแลระบบ**

    ---

    Backup, Troubleshooting
    และอัปเกรดเวอร์ชันอย่างปลอดภัย

    [:octicons-arrow-right-24: ดูแลระบบ](23-backup.md)

-   :material-clipboard-list:{ .lg .middle } **ภาคผนวก**

    ---

    Config พร้อมใช้ คำสั่ง CLI
    ตารางเทียบ Detector และ Checklist

    [:octicons-arrow-right-24: เปิดภาคผนวก](appendix-a.md)

</div>

---

## เหมาะกับใคร

- [x] คนที่อยากทำกล้องวงจรปิดใช้เอง ไม่พึ่ง Cloud
- [x] ผู้ใช้ Home Assistant ที่อยากเพิ่มระบบกล้อง
- [x] คนที่มี NAS / มินิพีซี อยู่แล้วอยากใช้ให้คุ้ม
- [x] มือใหม่ที่ไม่เคยแตะ Docker มาก่อน

---

!!! warning "ก่อนเริ่ม"
    เนื้อหาอ้างอิง Frigate เวอร์ชันล่าสุด บาง option อาจต่างกันในเวอร์ชันเก่า
    ตรวจสอบเวอร์ชันของคุณก่อนคัดลอก config ไปใช้
