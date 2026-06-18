#http methods (วิธีการของ HTTP)

-GET: ร้องขอข้อมูลจากทรัพยากรที่ระบุ
-POST: ส่งข้อมูลไปยังทรัพยากรที่ระบุ เพื่อประมวลผลหรือสร้างข้อมูลใหม่
-PUT: อัปเดตหรือแทนที่ทรัพยากรที่ระบุทั้งหมด
-DELETE: ลบทรัพยากรที่ระบุ
-PATCH: อัปเดตทรัพยากรที่ระบุเพียงบางส่วน
-HEAD: ร้องขอเฉพาะข้อมูลส่วนหัว (metadata) ของทรัพยากรที่ระบุ
-OPTIONS: อธิบายตัวเลือกการเชื่อมต่อสำหรับทรัพยากรเป้าหมาย
-TRACE: ทำการทดสอบส่งข้อมูลย้อนกลับ (loop-back) ตามเส้นทางไปยังทรัพยากรเป้าหมาย
-CONNECT: สร้างการเชื่อมต่อแบบอุโมงค์ (tunnel) ไปยังเซิร์ฟเวอร์ที่ระบุโดยทรัพยากรเป้าหมาย
-OPTIONS
-TRACE
-CONNECT
 
 #status (รหัสสถานะ HTTP)
 - 200 OK: คำร้องขอสำเร็จเรียบร้อย
 - 201 Created: คำร้องขอสำเร็จและมีการสร้างทรัพยากรใหม่แล้ว
 - 204 No Content: คำร้องขอสำเร็จ แต่ไม่มีเนื้อหาข้อมูลส่งกลับมา
 - 301 Moved Permanently: ทรัพยากรถูกย้ายไปยัง URL ใหม่เป็นการถาวร
 - 400 Bad Request: คำร้องขอไม่ถูกต้อง (รูปแบบไม่ถูกต้องจากฝั่ง Client)
 - 401 Unauthorized: ไม่ได้รับอนุญาต (ต้องยืนยันตัวตนก่อน)
 - 403 Forbidden: ปฏิเสธการเข้าถึง (ไม่มีสิทธิ์เข้าถึง)
 - 404 Not Found: ไม่พบทรัพยากรที่ร้องขอ
 - 500 Internal Server Error: เกิดข้อผิดพลาดภายในเซิร์ฟเวอร์
 - 503 Service Unavailable: เซิร์ฟเวอร์ไม่พร้อมให้บริการ (เช่น ปิดปรับปรุงชั่วคราว)

#cookies
# MySite2026

## การสร้างโปรเจกต์

    mkdir mysite2026
    cd mysite2026
    uv init
    uv add django
    uv run django-admin startproject mysite2026 .

## คำสั่งที่ใช้

    uv run manage.py runserver 0.0.0.0:80
    uv run manage.py startapp core

## คำสั่ง git
    git config --global user.name "thesombats"
    git config --global user.email "thesombats@gmail.com"

    git add .
    git commit -m "add project"
    git push origin main

## http methods 

- GET ใช้รับข้อมูล
- POST ใช้ส่งข้อมูล
- PUT ใช้แก้ไขข้อมูล
- DELETE ใช้ลบข้อมูล
- PATCH ใช้แก้ไขข้อมูลบางส่วน

## http status code

- 200 OK รับข้อมูลสำเร็จ
- 201 Created สร้างข้อมูลสำเร็จ
- 204 No Content ลบข้อมูลสำเร็จ
- 400 Bad Request ส่งข้อมูลไม่ถูกต้อง
- 401 Unauthorized ไม่ได้ล็อกอิน
- 403 Forbidden ไม่ได้รับอนุญาต
- 404 Not Found ไม่พบข้อมูล
- 500 Internal Server Error เซิฟเวอร์มีปัญหา
