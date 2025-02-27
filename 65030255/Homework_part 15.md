# 65030255
# Lab-01  ชนิดข้อมูลตัวเลขจำนวนเต็ม (Integer Types)

ข้อมูลชนิดตัวเลขจำนวนเต็ม สามารถนำไปใช้งานได้หลากหลาย เช่น การนับหรือแสดงจำนวน การกำหนดลำดับที่ การจัดลำดับ เป็นต้น ค่าที่ใส่ลงในตัวแปร เป็นได้ทั้งค่าบวก ค่าศูนย์ และค่าลบ (มีตัวแปรบางชนิดที่เก็บเฉพาะค่าบวกเพียงอย่างเดียว) การกำหนดค่าใดๆ ให้กับตัวแปร ทำได้โดยการใช้เครื่องหมาย =
การใช้เครื่องหมายคณิตศาสตร์กับตัวแปรจำนวนเต็ม สามารถใช้ได้ทุกเครื่องหมาย ได้แก่ +, -, *, / และ %

## 15. การใช้เครื่องหมายทางคณิตศาสตร์กับตัวแปรชนิดจำนวนเต็ม

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
int a, b, c, d, e, f;
a = 1;
b = a + 6;
c = b - 3;
d = c * 2;
e = d / 2;
f = e % 2;
Console.WriteLine("a={0}", a);
Console.WriteLine("b={0}", b);
Console.WriteLine("c={0}", c);
Console.WriteLine("d={0}", d);
Console.WriteLine("e={0}", e);
Console.WriteLine("f={0}", f);
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/875cf6ad-1930-4fdd-b4bc-4363c74dcbb9)

## 16. หาค่าจากสมการทางคณิตศาสตร์

กำหนด ```a = 10, b = 20, x = 5, y = 2``
👉 ให้เขียนโปรแกรมเพื่อหาผลลัพธ์ของสมการต่อไปนี้

1. `a+b`
2. `x-b`
3. `x*b`
4. `y/a`
5. `b%y`
6. `y+10%x`
7. `a/3*5`
8. `9/2*a`
9. `y%8`
10. `100*x+y%2-a`

```csharp
int a = 10, b = 20, x = 5, y = 2;
Console.WriteLine("a + b = " + (a + b));
Console.WriteLine("x - b = " + (x - b));
Console.WriteLine("x * b = " + (x * b));
Console.WriteLine("y / a = " + (y / (double)a));  
Console.WriteLine("b % y = " + (b % y));
Console.WriteLine("y + 10 % x = " + (y + 10 % x));
Console.WriteLine("a / 3 * 5 = " + (a / 3 * 5));
Console.WriteLine("9 / 2 * a = " + (9 / 2 * a));
Console.WriteLine("y % 8 = " + (y % 8));
Console.WriteLine("100 * x + y % 2 - a = " + (100 * x + y % 2 - a));
```

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/38fa539b-0c9d-4349-9133-33aa93a5fe2a)


## ชนิดข้อมูลเลขทศนิยม (Floating Point and Decimal Types)

ตัวเลขจำนวนทศนิยม มักจะใช้ในการคำนวณทางวิทยาศาสตร์ เนื่องจากค่าในวิทยาศาสตร์ต้องการความละเอียดสูง หรือมีค่าสูงมากกว่าที่เลขจำนวนเต็มจะเก็บได้

### ตัวอย่างการแก้ปัญหาทางวิทยาศาสตร์

ระยะทางจากดาวอาทิตย์ถึงโลกคือ 93,000,000 ไมล์ เรียกว่า 1 A.U. (Astronomical Unit)
ความเร็วในการเดินทางของแสงคือ 186,000 ไมล์ต่อวินาที
ระยะทาง 1 ไมล์ คิดเป็น 1.609344 กิโลเมตร
ให้เขียนโปรแกรมหาระยะทางในการเดินทางของแสง ในหน่วยกิโลเมตรต่อวินาทีและเวลาในการเดินทางของแสงจากดวงอาทิตย์มายังโลก

## 17.  โปรแกรมคำนวณระยะทางและเวลาของแสงจากดวงอาทิตย์ถึงโลก

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
const double lightSpeed = 186000d;   // miles per second
Console.WriteLine("Light speed = {0} Mile Per second", lightSpeed);
const double mileTokm = 1.609344;
Console.WriteLine("Light speed = {0} km Per second", lightSpeed*mileTokm);
const double SunToEarthDistance =  93000000d ;  // miles
Console.WriteLine("SunToEarthDistance = {0} km", SunToEarthDistance * mileTokm);
double SunToEarthTimeOfLight = SunToEarthDistance / lightSpeed;  // miles
Console.WriteLine("SunToEarthTimeOfLight = {0} seconds", SunToEarthTimeOfLight);
Console.WriteLine("SunToEarthTimeOfLight = {0} minutes", SunToEarthTimeOfLight/60d);
```

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/fd2b21dd-0b6f-4f46-a7c6-c9e9cbd5da9a)


👷 คำสั่ง ให้เขียนโปรแกรมคำนวณค่าเพื่อเติมลงในช่องว่างในตาราง
ตารางที่ 1 ระยะทางจากดวงอาทิตย์ถึงดาวเคราะห์ต่างๆ

| ดาวเคราะห์  | ระยะทางจากดวงอาทิตย์ (km) | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที) |
|--------------|------------------------|------------------------|------------------------|
| Mercury      | 57,910,000             |      0.387098            |         3.223437           |
| Venus        | 108,200,000           |      0.723331            |         5.984475           |
| Earth        | 149,600,000           |      1.000000            |         8.317122           |
| Mars         | 227,940,000           |      1.523688            |        12.555248          |
| Jupiter      | 778,330,000           |      5.203363            |        43.268936          |
| Uranus       | 2,873,550,000        |     19.218446           |       159.778796         |
| Neptune      | 4,501,000,000        |     30.047098           |       249.742063         |
| Pluto        | 5,945,900,000        |     39.482116           |       327.669856         |




 คลาส Math ในภาษา C# มีคลาสที่เป็นตัวช่วยคำนวณทางคณิตศาสตร์ ที่ช่วยให้เราสามารถคำนวณฟังก์ชันพื้นฐานได้ อย่างรวดเร็ว ไม่ต้องพัฒนาโปรแกรมเพิ่มเติมด้วยเอง นั่นคือคลาส Math ฟังก์ชันทางคณิตศาสตร์ที่ใช้บ่อยๆ สามารถดูรายละเอียดทั้งหมดได้จาก `system.math`

```csharp
double distanceToEarthAU = CalculateAU(149600000);
double distanceToMercuryAU = CalculateAU(57910000);
double distanceToVenusAU = CalculateAU(108200000);
double distanceToMarsAU = CalculateAU(227940000);
double distanceToJupiterAU = CalculateAU(778330000);
double distanceToUranusAU = CalculateAU(2873550000);
double distanceToNeptuneAU = CalculateAU(4501000000);
double distanceToPlutoAU = CalculateAU(5945900000);
//-----------------------------------------------------------------------
double timeToMercuryMinutes = CalculateLightTime(57910000);
double timeToVenusMinutes = CalculateLightTime(108200000);
double timeToEarthMinutes = CalculateLightTime(149600000);
double timeToMarsMinutes = CalculateLightTime(227940000);
double timeToJupiterMinutes = CalculateLightTime(778330000);
double timeToUranusMinutes = CalculateLightTime(2873550000);
double timeToNeptuneMinutes = CalculateLightTime(4501000000);
double timeToPlutoMinutes = CalculateLightTime(5945900000);

Console.WriteLine("| ดาวเคราะห์  | ระยะทางในหน่วย A.U. | เวลาของแสง (นาที) |");
Console.WriteLine("|--------------|------------------------|------------------------|");
Console.WriteLine($"| Mercury      | {distanceToMercuryAU,23:F6} | {timeToMercuryMinutes,23:F6} |");
Console.WriteLine($"| Venus        | {distanceToVenusAU,23:F6} | {timeToVenusMinutes,23:F6} |");
Console.WriteLine($"| Earth        | {distanceToEarthAU,23:F6} | {timeToEarthMinutes,23:F6} |");
Console.WriteLine($"| Mars         | {distanceToMarsAU,23:F6} | {timeToMarsMinutes,23:F6} |");
Console.WriteLine($"| Jupiter      | {distanceToJupiterAU,23:F6} | {timeToJupiterMinutes,23:F6} |");
Console.WriteLine($"| Uranus       | {distanceToUranusAU,23:F6} | {timeToUranusMinutes,23:F6} |");
Console.WriteLine($"| Neptune      | {distanceToNeptuneAU,23:F6} | {timeToNeptuneMinutes,23:F6} |");
Console.WriteLine($"| Pluto        | {distanceToPlutoAU,23:F6} | {timeToPlutoMinutes,23:F6} |"); //ก็ในเว็บเขียน 6 ตำแหน่งเลยเอา F6

static double CalculateAU(double distanceToSun)
{
    return distanceToSun / 149600000;
}
static double CalculateLightTime(double distanceToSun)
{
    double speedOfLight = 299792;
    return distanceToSun / speedOfLight;
}

```
 
## 20.  โปรแกรมพล็อตรูป sine wave บนหน้าจอ

👉 ให้เขียนโปรแกรมต่อไปนี้

```csharp
for (float i = 0; i < Math.PI * 2.0F; i += 0.3F)
{
    Console.WriteLine("The sine of {0,10:F} = {1,-10:F6}" + spaces(Math.Sin(i)) + "*", i, Math.Sin(i));
}
string spaces(double val)
{
    string SpaceString = new String(' ', ((int)(val * 10.0)) + 10);
    return SpaceString;
}
```

หมายเหตุ ในการเขียนโปรแกรมภาษา C# .NET6.0 ที่ใช้ template แบบใหม่ เราก็ยังคงสามารถสร้าง function ใช้งานได้ตามปกติ (แต่จะไม่ครอบคลุม feature ทั้งหมดใน OOP )

➢ รันโปรแกรมและบันทึกผล

![image](https://github.com/Sorawit255/03376836-OOP-2566-Lab-01/assets/144196505/b33936ec-0f31-45db-bb0d-fc435c424c4e)


  
