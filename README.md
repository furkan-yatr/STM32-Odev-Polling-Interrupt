# STM32 Gömülü Sistem Ödevi

Bu proje kapsamında aşağıdaki 4 temel adım uygulanmıştır:

1. [cite_start]**Buton Girişinin Okunması:** Polling ve Interrupt yöntemleriyle buton durumu okunmuştur[cite: 80, 123].
2. **Yöntem Karşılaştırması:**
| Özellik | Polling | Interrupt |
| :--- | :--- | :--- |
| CPU Kullanımı | [cite_start]Yüksek (Sürekli kontrol) [cite: 119] | [cite_start]Düşük (Sadece olayda) [cite: 119] |
| Enerji Verimliliği | [cite_start]Düşük [cite: 119] | [cite_start]Daha Yüksek [cite: 119] |
| Tepki Süresi | [cite_start]Gecikmeli olabilir [cite: 120] | [cite_start]Çok hızlı [cite: 120] |
| Karmaşıklık | [cite_start]Basit [cite: 120] | [cite_start]Daha karmaşık [cite: 120] |

3. [cite_start]**Harici Kesme (EXTI) Yapılandırması:** CubeMX üzerinden tetikleme türü ve NVIC ayarları yapılmıştır[cite: 129, 133, 140].
4. [cite_start]**Gerçek Zamanlı Olay Tespiti:** ISR (Interrupt Service Routine) fonksiyonu ile butona basıldığı an LED durumu değiştirilmiştir[cite: 142, 160].
