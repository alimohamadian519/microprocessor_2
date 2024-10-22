# آزمایش 1 

## گزارش کار

هدف راه اندازی دو LED چشمک زن می باشد به طوری که یکی روشن و دیگری خاموش باشد و خلاف یکدیگر چشمک بزنند.

---

### کد برنامه 

```cpp
int led1 = 13;
int led2 = 7;

void setup() {
pinMode(led1, OUTPUT);
pinMode(led2, OUTPUT);
}

void loop() {
digitalWrite(led1, HIGH);   
digitalWrite(led2, LOW);
delay(1000);
digitalWrite(led1, LOW);
digitalWrite(led2, HIGH);   
delay(1000);
}
```

---

### عکس مدار


![micro and circuit](/pic/microprocessor_2.jpg)

---

### شماتیک مدار

![schematic](/media/schematic_1.jpg)
