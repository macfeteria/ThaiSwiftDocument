# Thai Swift Document
The Swift Programming Language (Thai translation)

# Swift 3.0
เอกสารแปลงจากไฟล์ epub เป็น xhtml ดังนั้นแล้วสามารถใช้ html editor แก้ไขได้ทันที
หนังสือเล่มนี้แปลจาก The Swift Programming Language , Swift 3 Edition (Beta)

# How to contribute
โปรเจคนี้เป็นของชุมชนนักพัฒนาภาษา Swift ในไทย, Swift Thailand User Group :)
คุณสามารถมีส่วนร่วมแปลภาษาได้ด้วยการ

- แปลบทความ
- ร่วมตรวจสอบคำและไวยกรณ์ต่างๆ
- เรียบเรียงภาษา


## Start translation

เนื่องจากว่ามีคนหลายคนทำงานบนโปรเจคนี้ ซึ่งแน่นอนว่าอาจจะมีคนแปลบทความเดียวกันกับคุณ
ฉะนั้นแล้ว ก่อนที่จะลงมือแปล ให้ตรวจสอบ issue ในหน้า
https://github.com/macfeteria/thai-swift-document/issues
เสียก่อนว่ามีใครเริ่มลงมือแปลส่วนใดบ้าง  หากไม่พบว่ามีคนแปลบทความที่คุณกำลังจะเริ่มแปล ก็ให้สร้าง issue ใหม่ พร้อมกับบอกรายละเอียดด้วยว่าคุณกำลังเริ่มต้นแปล บทใด , ส่วนใด
แต่ถ้าหาก พบว่ามีคนกำลังแปล บทความเดียวกัน ให้สอบถามที่ issue นั้นว่าส่วนใดยังไม่ได้เริ่มแปล เพื่อที่จะได้ไม่เป็นการเสียเวลาทำงานซ้ำซ้อนกัน

## Basic Git

หากคุณยังไม่เคยร่วมกับ opensource project ใดๆ นี่เป็นโอกาสที่ดี
ที่คุณจะได้มีส่วนช่วยพัฒนาชุมชน Swift ในไทย

ถ้าหากไม่เคยใช้งาน git มาก่อน ขอแนะนำวิธีการเบี้องต้นในการเริ่มต้นแปลบทความ
#### Folk & Clone
1. กดปุ่ม fork ที่อยู่ทางด้านขวามือหน้าเวป github
2. หลังจากนั้นคุณก็จะมีก๊อปปี้ของโปรเจคนี้อยู่ที่ git account ของตัวเอง เช่น
https://github.com/you-git-account/thai-swift-document
3. เปิด terminal เพื่อใช้งาน git command
4. ทำการ clone โปรเจคจาก git account ของตัวเองมาไว้ที่เครื่อง ด้วยคำสั่ง
git clone https://github.com/you-git-account/thai-swift-document
ตอนนี้คุณก็มีโปรเจคอยู่ที่เครื่องของตัวเองเรียบร้อยแล้ว
5. สร้าง develop branch ใหม่ด้วยคำสั่ง
git branch develop
6. เพื่อเปลี่ยนไปยัง branch ที่เพิ่งได้สร้างไปด้วยคำสั่ง
git checkout develop
7. เพิ่ม remote ด้วยคำสั่ง
git remote add upstream https://github.com/macfeteria/thai-swift-document
8. ตรวจสอบว่า remote นั้นถูกต้องด้วยคำสั่ง git remote -v ซึ่งจะเห็นรายละเอียดดังนี้

- origin	https://github.com/you-git-account/thai-swift-document (fetch)
- origin	https://github.com/you-git-account/thai-swift-document (push)
- upstream	https://github.com/macfeteria/thai-swift-document.git (fetch)
- upstream	https://github.com/macfeteria/thai-swift-document.git (push)

8. พิมพ์คำสั่ง git remote update เพื่ออัพเดทข้อมูล
9. พิมพ์คำสั่ง git pull upstream master ดึงข้อมูลล่าสุดมาไว้เครื่องตัวเอง
10. เท่านี้คุณก็พร้อมแล้ว

#### Push your change.

1. หลังจากที่คุณแปลเสร็จแล้ว ก็ให้ทำการ commit สิ่งที่ได้แก้ไขไป พร้อมกับรายละเอียดว่าได้ทำอะไรไปบ้าง ด้วยคำสั่ง

git commit * -m "แก้ไขบทที่ 1 เพิ่มการใช้งานตัวแปร"

เนื่องจากมีคนทำงานหลายคน ดังนั้นแล้วเมื่อคุณแปลเสร็จ ข้อมูลที่คุณมี ณ เวลาที่คุณทำงานเสร็จ อาจจะไม่ใช่ข้อมูล่าสุด ดังนั้นจึงต้องดึงข้อมูลล่าสุดของโปรเจค เข้ามารวมกับสิ่งที่ได้ตัวเองแก้ไขไป

2. พิมพ์คำสั่ง git pull upstream master
3. หากเกิด conflict ให้แก้ไขเสียก่อน แล้ว commit เอกสารใหม่ที่ได้แก้ไข conflict ไป
4. หากไม่มี conflict หรือแก้ไข conflict เสร็จแล้วพิมพ์คำสั่ง
git rebase develop
5. ส่งโค้ดขึ้น github ด้วยการพิมพ์คำสั่ง
git push origin develop
ณ ตอนนี้คุณได้ส่งเอกสารที่ได้แก้ไปยัง git account ของคุณแล้ว

#### Pull request.
ในลำดับต่อไป คือการขอ pull request เพื่อให้รวมเอาข้อมูลที่คุณได้แก้ไขไป รวมเข้ากับ โปรเจคหลัก
1. กดสร้าง pull request จากหน้าเวป เพื่อขอนำเอาสิ่งที่คุณได้ทำไป ไปรวมเข้ากับโปรเจค พร้อมกับบอกรายละเอียดต่างๆที่ได้แก้ไขไป
2. หากทุกอย่างโอเค สิ่งที่คุณได้แก้ไขไปก็จะถูกรวมเข้าไปยังโปรเจค :)

ปล. แน่นอนว่า ทุกๆอย่างในนี้แก้ไขและปรับปรุงให้ดีขึ้นได้ แม้กระทั่ง readme.md ไฟล์นี้
