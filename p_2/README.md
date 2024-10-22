# آزمایش2

## گزارش کار

هر دو LED همزمان 5 ثانیه روشن و سپس نیم ثانیه خاموش می شوندو دوباره این مراحل تکرار میشود. دو LEDهر کدام به یک خروجی متفاوت از برد آردوینو متصل شدند و مجزا ازهم کار می کنند  

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
digitalWrite(led2, HIGH);   
delay(5000);
digitalWrite(led1, LOW);
digitalWrite(led2, LOW);    
delay(500);
}
```

---

### عکس مدار

![micro and circuit](/media/microprocessor_3.gif)

---

### شماتیک مدار

![schematic](/media/schematic_1.jpg)
