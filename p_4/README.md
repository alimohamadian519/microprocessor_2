# آزمایش4

## گزارش کار

برنامه ای میخواهیم بنویسیم که کاراکتر مشخصی از ورودی serial monitor بخواند. با وارد کردن یه کاراکترمثلا(h) ledروشن وبا وارد کردن کارکتر دیگرمثلا(l) led خاموش شود.

---

### کد برنامه

```cpp
const int led = 8;  

void setup() {
  pinMode(led, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  if (Serial.available() > 0) { 
    char inputLed = Serial.read();  
    if (inputLed == 'h' || inputLed == 'H') {
      digitalWrite(led, HIGH);
    } else if (inputLed == 'l' || inputLed == 'L') {    
      digitalWrite(led, LOW);
    }
  }
}
```

---

### شماتیک مدار 

![schematic](/media/schematic_2.jpg)
