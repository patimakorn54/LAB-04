# นายปฏิมากร บุญเปลี่ยน 57030190
#ใบงานที่ 4 เรื่อง การใช้งานคำสั่งเกี่ยวกับการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C#
##วัตถุประสงค์
1. เพื่อให้นักศึกษาบอกชื่อ method ที่ใช้ในการแสดงผลบน Text Mode ขั้นพื้นฐานในภาษา C# ได้
2. เพื่อให้นักศึกษาสามารถใช้คำสั่งแสดงผลทางหน้าจอ เบื้องต้นได้

##ลำดับขั้นการทดลอง
###การเตรียมการก่อนการทดลอง
  * เปิดโปรแกรม Visual Studio 
  *  เลือก File >>New Project >> เลือก Console Application 
![P1](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P1.png)
  *  ช่อง Name ใส่ชื่อของ project (ในที่นี้คือ Lab4)
  *  ช่อง Location ใส่ชื่อ folder ที่เป็นที่ตั้งของ Project (ในที่นี้ สมมติเป็น E:\vslab)
  *  ช่อง Solution name ให้ใส่ชื่อ Solution โดยปกติก็ให้ปล่อยไว้อย่างนั้น 
  *  กดปุ่ม OK โปรแกรม Visual Studio จะสร้าง project ชื่อ “lab4”ภายใต้ solution “lab4” และไฟล์ lsb4.cs ซึ่งมี source code ดังรูป 

![P2](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P2.png)

ส่วนสำคัญของโปรแกรม lab4.cs  คือบรรทัดที่ 1 “using System” และเมธอด Main(string[] args)


 *  ให้ลบ source code ในบรรทัดที่ 2-5 ออกไปก่อน เนื่องจากเป็น assembly ที่ไม่จำเป็นต่อการทำงานของโปรแกรม 

## 1. การทดลองเมดธอด Console.Write()
* ให้เพิ่ม บรรทัดต่อไปนี้ลงไปในในเมธอด Main()
```csharp 
    Console.Write(“Hello”);
```
ดังปรากฏในบรรทัดที่ 9 ของรูปด้านล่าง 

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P3.png)
 
 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

####บันทึกผลการทดลอง
จากการทดลองพบว่า จะขึ้นข้อความ Hello

![](https://github.com/patimakorn54/LAB-04/blob/master/imgs/Capture1.JPG?raw=true)

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้    

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P4.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม
 * การรันแล้วทำให้หน้าจอ console ยังคงแสดงผลค้างอยู่นั้น ให้เลือกเมนู Debug -> Start Without Debugging (Ctrl+F5) มิฉะนั้น หน้าจอ console จะหายไปอย่างรวดเร็ว

![](https://github.com/patimakorn54/LAB-04/blob/master/imgs/Capture2.JPG?raw=true)


### คำถาม 4.1 

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย


ไม่ เพราะว่าข้อความ HelloWorld ติดกัน


## 2. การทดลองเมดธอด Console.WriteLine()

แก้โปรแกรมในเมดธอด Main() ให้เป็นดังรูปต่อไปนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P5.png)

 * สั่ง Run โปรแกรม เพื่อดูผลการทดลอง 

![](https://github.com/patimakorn54/LAB-04/blob/master/imgs/Capture3.JPG?raw=true)

บันทึกผลที่ได้จากการรันโปรแกรม


จากการทดลองพบว่า เมื่อเปลี่ยนจากคำว่า Write เป็น WriteLine จะทำให้เกิดการเลื่อนบรรทัดลงมา

แก้ไขโปรแกรม ให้เป็นดังรูปด้านล่างนี้

![](https://github.com/Desktop-Programming-Lab-2559/LAB-04/blob/master/imgs/P6.png)

 * สั่ง Run โปรแกรมและบันทึกผลที่ได้จากการรันโปรแกรม

![](https://github.com/patimakorn54/LAB-04/blob/master/imgs/Capture4.JPG?raw=true)


จากการทดลองพบว่าเมื่อ เปลี่ยนจากคำว่า Write เป็น WriteLine จะทำให้เกิดการเลื่อนบรรทัดลงมา


###คำถาม 4.2

ผลที่ได้จากการทดลอง เป็นอย่างที่นักศึกษาคิดหรือไม่ อย่างไร  จงอธิบาย


เป็น เพราะว่า เกิดการเว้นบรรทัดลงมา

### คำถาม 4.3 

จงอธิบายความแตกต่างระหว่างคำสั่ง Console.Write() และ Console.WriteLine()

Write คือการแสดงผลแบบข้อความต่อกัน ส่วน WriteLine คือการแสดงข้อความแบบเว้นบรรทัดลงมา



##สรุปผลการทดลอง

ถ้าต้องการให้ตัวอักษรต่อกันให้ใช้ Write แต่ถ้าต้องการการเว้นบรรทัดให้ใช้คำสั่ง WriteLine

