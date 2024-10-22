## آزمایش6

## گزارش کار

اگر کاربر یک عدد صحیح وارد کرد LED روشن و بلعکس.مثلا عدد 101 معادل روشن و عدد 201 معادل خاموش می باشد.

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
    int inputLed = Serial.parseInt();   
    if (inputLed == 101) {
      digitalWrite(led, HIGH);
    } else if (inputLed == 201) {
      digitalWrite(led, LOW);
    }
  }
}
```

---

### شماتیک مدار

![schematic](/media/schematic_2.jpg)
