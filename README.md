> แก้ไขครั้งล่าสุด: 11/07/2019 เวลา 19.06 น.

YRC Internet Authenticator
----------
UI Design ตัวนี้ เป็นผลงานตัวแรกของผมที่มีการนำไปใช้จริง โดยได้รับคำร้องขอมาจาก คุณครูวิรัชชัย จันต๊ะวงศ์ ให้ดำเนินการออกแบบ UI แทนที่ตัวเดิมที่ใช้งานมานาน ทั้งนี้ เป็นเพราะการแสดงผลของเว็บไซต์บนหน้าจอที่เปลี่ยนไป ทำให้ UI แบบเก่าไม่รองรับการแสดงผลบนอุปกรณ์จอขนาดเล็ก เช่น Smartphone ได้ ผมจึงมีความสนใจที่จะพัฒนา UI ใหม่ ตามหลัก mobile-first design เพื่อให้ UI ตัวนี้รองรับกับทุกอุปกรณ์ ทั้งยังเพิ่มความสะดวกสบายต่อการใช้งาน และเป็นภาพลักษณ์ที่ดีต่อโรงเรียนยุพราชวิทยาลัย ในฐานะของศูนย์โอลิมปิกวิชาการคอมพิวเตอร์อีกด้วย

หากสนใจดูตัวอย่าง สามารถเข้าไปที่ https://dward2nd.github.io/yrc-internet-authenticator โดยผมจะเปิด repo นี้เป็นสาธารณะเพื่อให้รุ่นน้อง หรือผู้ที่สนใจได้ลองศึกษา

Implementation
---------
ออกแบบไว้เฉพาะส่วนที่เป็น front-end เท่านั้น เพราะทาง back-end นั้นจะมีครูที่ดูแลเรื่องนี้โดยเฉพาะ ซึ่งผมไม่มีสิทธิ์เข้าถึงส่วนนั้น

> CSS Famework ที่ใช้: Bulma

สาเหตุที่เลือก
-------

ตอนแรกผมจะใช้ Bootstrap แล้วครับ แต่ผมตระหนักถึงประสิทธิภาพของการโหลด ที่ควรกินเวลานานน้อยที่สุด และใช้หน่วยความจำให้น้อยที่สุด (แต่ยังคงความสวยงามไว้บ้าง) ผมจึงเลือกใช้ Bulma เพราะเป็น CSS Framework ที่เบากว่า Bootstrap มาก เน้นไปที่การออกแบบ มากกว่าจะเป็นฟังก์ชัน และสำหรับรูปที่ใช้มีการปรับทั้งขนาดและตัดต่อก่อนที่จะนำมาใช้ เพื่อหลีกเลี่ยงการใช้ filter ใน CSS จึงทำให้รูปโหลดได้เร็ว และ animation ลื่นไหลมาก
