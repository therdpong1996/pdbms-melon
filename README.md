# PDBMS-MELON
Source ESP8266 Code and Website Code for PDBMS-Melon

## วิธีติดตั้ง

**Import ไฟล์ SQL เข้า Database**

**เปิดไฟล์ init.php มาแก้ไข**
- เปลี่ยน `{{host}}` เป็น localhost หรือ IP ของ Database
- เปลี่ยน `{{dbname}}` เป็นชื่อ Database ที่ Import ไฟล์ SQL เข้า
- เปลี่ยน `{{username}}` เป็นชื่อผู้ใช้ของฐานข้อมูล
- เปลี่ยน `{{password}}` เป็นรหัสผ่านของฐานข้อมูล
- เปลี่ยน `{{wsurl}}` เป็น URL ของเว็บไต์ (ต้องมี https:// และ / ปิดท้าย)
- เปลี่ยน `{{imgpass}}` เป็นรหัสผ่านสำหรับอัพโหลดรูปภาพ
- เปลี่ยน `{{fburl}}` เป็น URL ของ Firebase (ต้องมี https://)
- เปลี่ยน `{{imgwidth}}` เป็นขนาดความกว้างของรูปภาพที่อัพโหลด (แนะนำ 512) (สูงสุด 1024)
- เปลี่ยน `{{imgheight}}` เป็นขนาดความสูงของรูปภาพที่อัพโหลด (แนะนำ 512) (สูงสุด 1024)
- เปลี่ยน `{{imgqua}}` เป็นคุณภาพ (ความละเอียด) ของรูปภาพที่อัพโหลดเป็น % (แนะนำ 80) (สูงสุด 100)

## วิธีใช้งาน (ใช้ Method GET)
- http(s)://`<domain-name>`/insert/?temp=`<temp>`&humi=`<humi>`&light=`<light>`&weight=`<weight>`&mosi=`<mosi>`
