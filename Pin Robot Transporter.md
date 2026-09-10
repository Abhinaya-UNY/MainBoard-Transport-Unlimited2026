# Pin Robot Transporter

---

## 1. Komunikasi Serial (UART)

| Modul                   | Pin RX    | Pin TX    | Keterangan |
| ----------------------- | --------- | --------- | ---------- |
| **ESP32-WROOM-32U**     | 16 (RX2)  | 17 (TX2)  |  UART2     |
| **STM32f103c8t6**       | PA3 (RX2) | PA2 (TX2) |  USART2    |

---

## 2. Motor Driver (STM32f103c8t6 Blue Pill)

| Komponen         | Arah (Pin Driver) |   Pin STM32  | Hardware Timer       |
| :--------------- | :---------------- | :----------: | :------------------- |
| **Motor 1 (M1)** | IN1<br>IN2        |  PB8<br>PB9  | TIM4_CH3<br>TIM4_CH4 |
| **Motor 2 (M2)** | IN1<br>IN2        |  PB6<br>PB7  | TIM4_CH1<br>TIM4_CH2 |
| **Motor 3 (M3)** | IN1<br>IN2        | PA10<br>PA11 | TIM1_CH3<br>TIM1_CH4 |
| **Motor 4 (M4)** | IN1<br>IN2        |  PA8<br>PA9  | TIM1_CH1<br>TIM1_CH2 |
| **Motor 5 (M5)** | F<br>B            |  PA1<br>PA0  | TIM2_CH2<br>TIM2_CH1 |

---

## 3. Servo

| Komponen         | Label Pin  | Pin ESP32 |
| :--------------- | :--------- | :-------- |
| **Servo 1 (S1)** | Signal (S) | 32        |
| **Servo 2 (S2)** | Signal (S) | 33        |
| **Servo 3 (S3)** | Signal (S) | 25        |
| **Servo 4 (S4)** | Signal (S) | 26        |

---

## 4. Sensor

| Komponen           | Fungsi / Jalur           | Pin ESP32            | Keterangan                      |
| :----------------- | :----------------------- | :------------------- | :------------------------------ |
| **MPU 6050**       | SDA<br>SCL<br>AD0<br>INT | 21<br>22<br>19<br>18 | Sensor IMU (Gyro/Accelerometer) |
| **BNO085**         | SDA<br>SCL<br>INT<br>RST | 21<br>22<br>19<br>18 | Sensor Orientasi Absolut        |
| **ID-BAT**         | OUT                      | 35                   | Indikator / Pembacaan Baterai   |
| **Current Sensor** | OUT                      | 34                   | Pembacaan Arus (Input Analog)   |
| **LED Strip**      | OUT                      | 13                   | indikator banyak hal            |
| **Laser**          | Switch                   | 4                    | Laser on/of                     |

---

## 5. Encoder (SPI1)

| Komponen       | Fungsi / Jalur | Pin STM32 | Hardware Timer |
| :------------- | :------------- | :-------- | :------------- |
| **Encoder 1**  | MISO           | PA6       | SPI1_MISO      |
|                | MOSI           | PA7       | SPI1_MOSI      |
|                | SCK            | PA5       | SPI1_SCK       |
|                | SS             | PA4       | SPI1_NSS       |
| **Encoder 2**  | MISO           | PA6       | SPI1_MISO      |
|                | MOSI           | PA7       | SPI1_MOSI      |
|                | SCK            | PA5       | SPI1_SCK       |
|                | SS             | PB13      | GPIO           |
| **Encoder 3**  | MISO           | PA6       | SPI1_MISO      |
|                | MOSI           | PA7       | SPI1_MOSI      |
|                | SCK            | PA5       | SPI1_SCK       |
|                | SS             | PB12      | GPIO           |

---
