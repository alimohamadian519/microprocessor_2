# آزمایش شماره5

## گزارش کار

یک ورودی را دریافت کرده و بر اساس آن  LED روشن و بلعکس.این دفعه رشته ای از کاراکترها می باشد مثلا ورودی کاراکترon روشن شدن led و OFF  باعث خاموش شدن آنled شود.

---

### کدبرنامه

```cpp
const int led = 8;

void setup() {
  pinMode(led, OUTPUT);
  Serial.begin(9600);
}

void loop() {
  if (Serial.available() > 0) {
    String inputLed = Serial.readString();  
    if (inputLed == 'on') {
      digitalWrite(led, HIGH);
    } else if (inputLed == 'off') {
      digitalWrite(led, LOW);
    }
  }
}
```

---

### شماتیک مدار 

![schematic](/media/schematic_2.jpg)
