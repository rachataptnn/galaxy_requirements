# Spaceship Repair Center

## Activities 

### User Management
- จะมี Activity ที่ใช้สำหรับเปิดโอกาสให้สิ่งมีชีวิต รวมถึง สิ่งไม่มีชีวิต ใดๆก็ตามที่มีปัญญา และ มีจริยธรรม มาจ่ายเงินให้เรา
- และ Activity นี้จะช่วยยืนยันว่าเราโอเคที่จะมี คุณๆท่านๆ เหล่านั้นเป็นลูกค้าของเรา
- เราต้องสามารถ Update Data ได้ เพราะอาจจะมี Scenario ย้ายที่อยู่อาศัย รวมถึงเราไม่อาจให้บริการกับลูกค้าบางท่านที่อาจจะไปก่ออาชญากรรมในอนาคต จนถูกหมายหัวจาก `ผู้พิทักษ์ Galaxy` 

![image](https://github.com/user-attachments/assets/41a0aa9a-44cd-46af-8e78-67538a30b0eb)

#### Possible Activity In this Feature
    - User Register
    - User Update
    - Delete User
    - Read User Detail
    - Read User List


### Spaceship Management
- `User` ที่ทำการสมัครสมาชิกเข้ามาแล้วต้องทำการระบุข้อมูลของยานด้วยการส่ง `central_spaceship_id` เข้ามาในระบบให้เราตรวจสอบ
- เราจะไปขอ `ข้อมูลของยานลำนั้น` กับ `องกรควบคุมและบันทึกพฤติกรรมการขับขี่ยานในระบบกาแล๊กซี่กลาง` 
- พอเรา Happy กับข้อมูลของยานลำนั้นแล้ว เราก็จะนำข้อมูลของยานจาก  มา store ลง Database เรา เพราะองกรนั้นคิดตังแต่ละ Transaction โคดแพง
- ด้วย Activity นี้เราจะประเมิณได้ว่า
    - ความเสี่ยงต่างๆของการรับยานมาซ่อม มีอะไรบ้าง (เอา central_spaceship_id ไป query หาประวัติของยานกับ )
    - เรามี Resource ในด้านต่างๆเพียงพอกับยานที่เขาจะเอามาซ่อม 
    - เราสามารถ suggest ข้อมูลต่างๆเช่น การปรับปรุงคุณภาพของระบบออกตัว, การขนส่งยาน, บริษัทประกันที่เหมาะสมกับลูกค้า

#### Possible Activity In this Feature
    - Spaceship inquiry with Central Spaceship Of Galaxy
    - Spaceship register
    - Spaceship scheduler update
    - Spaceship update
    - Spaceship delete
    - Spaceship Read Info
    - Spaceship Read List


### Booking Spaceship Fixing
- User ที่ต้องการ ซ่อม/ปรับปรุงยาน จะทำการสำรวจวันและเวลาที่สะดวกกับทางเราได้ด้วย Activity นี้
- Data Engineer ของเราจะใช้ Table นี้เป็น Main Data ในการ Forecast ทิศทาง และ ความเร็วในการเติบโตของธุรกิจการซ่อม
- การตัดเงินเมื่อ User Confirm payment เราจะใช้บริการ API กลางจาก `หน่วยงานแลกเปลี่ยนและซื้อขาย EA แห่ง NGC 1300` เนื่องจากราคางามความเสถียรใช้ได้ รวมถึงมี Currency ที่ทางเรารับแลกเปลี่ยนอยู่เกือบทุกชนิด

#### Possible Activity In this Feature
    - User Inquiry Booking
    - User Confirm Booking
    - User Payment
    - User Update Booking
    - User Delete Booking
    - User Read Booking Info
    - User Read Booking to Calendar
    - User Read Booking to Table


### Spare Part Management
- ใช้สำหรับบริหารจัดการอะไหล่ เชื้อเพลิง แร่ธาตุ ที่มีในคลัง เพื่อให้ระบบของเราสามารถทราบความเป็นไปได้ต่างๆ สำหรับการซ่อมยานลำที่ถูกจองเข้ามา

#### Possible Activity In this Feature
    - Spare Part Create
    - Spare Part Update
    - Spare Part Delete
    - Spare Part Read Detail
    - Spare Part Read List


### Technician Management
- ใช้สำหรับบริหารทรัพยากรบุคคลที่มีความรู้ความสามารถในด้านการซ่อมแซม วัตถุประสงของ Feature นี้ก็เหมือนข้อที่แล้ว
- เพื่อให้ระบบของเราสามารถทราบความเป็นไปได้ต่างๆ สำหรับการซ่อมยานลำที่ถูกจองเข้ามา
#### Possible Activity In this Feature
    - Technician Create
    - Technician Update
    - Technician Delete
    - Technician Read Detail
    - Technician Read List
