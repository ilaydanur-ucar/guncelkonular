# Güncel Konular Dersi 
# Safety 4.0 – CEOTHERM Homojenizasyon Tesisi

Güncel Konular dersi projesi. Safety 4.0 Bootcamp föylerindeki analizleri gerçek bir endüstriyel makineye uyguluyoruz: **CEOTHERM alüminyum biyet homojenizasyon tesisi.**

**Neden bu makine?** Tesis senkron çalışan 3 alt sistemden oluşuyor ve her birinin kendi **PLC + HMI**'ı var. Gaz, 580 °C ısı, hidrolik ve ağır yük de aynı yerde. Yani fonksiyonel emniyet ve OT siber güvenlik bir arada analiz edilebiliyor.

## Ekip
| İsim | Sorumluluk |
|---|---|
| ... | ... |

## Sistem

Homojenizasyon, alüminyum biyetleri ekstrüzyondan önce ~580 °C'de tavlama işlemi. Böylece biyet preste çatlamıyor ve alaşım elementleri homojen dağılıyor.

| Alt sistem | Öne çıkan özellikler |
|---|---|
| Homojenizasyon fırını | 580 °C, ±5 °C homojenlik, 8–11 saat ısıtma, doğal gazlı brülörler, motorlu kapı + pnömatik kilit, patlama kapakları, PLC + HMI |
| Soğutma kabini | Çift yönlü hava soğutma, 400 °C/saate kadar, PLC + HMI |
| Biyet transfer arabası | Kendi hidrolik ünitesi, fırın ve kabinle senkron, PLC + HMI |

> Not: Üreticinin TR ve EN sayfaları farklı değer veriyor. Kapasite 5–60 / 5–40 ton/şarj, gaz tüketimi <30 / <24 Nm³/ton.

**Hat içindeki yeri (çıkarım):**
Döküm → **Homojenizasyon → Transfer → Soğutma** → Testere → İstifleme → Ekstrüzyon

## SWOT

| | |
|---|---|
| **S – Güçlü yönler** | PLC + HMI ile reçete bazlı otomatik kontrol · ±5 °C homojenlik · patlama kapakları ve pnömatik kapı kilidi · düşük gaz tüketimi · modüler yapı |
| **W – Zayıf yönler** | 3 ayrı PLC/HMI = 3 saldırı yüzeyi · alt sistemler arası haberleşme manipülasyona açık · emniyet ve siber güvenlik dokümante edilmemiş · 8–11 saatlik proses yüzünden dar yama penceresi |
| **O – Fırsatlar** | Kestirimci bakım · enerji ve karbon izleme · güvenli uzak bakım · IEC 62443 uyumunu ihracat avantajına çevirmek · YZ destekli kalite kontrol |
| **T – Tehditler** | HMI veya uzak erişimden setpoint manipülasyonu · gaz yakma sistemine saldırı → patlama riski · fidye yazılımıyla hat duruşu · Makine Yönetmeliği 2023/1230 ve CRA yükümlülükleri · PLC/HMI bileşenlerindeki CVE'ler |

## Haftalık plan
| Hafta | Föy | Çıktı |
|---|---|---|
| 1 | Lab 1 – Safety Architecture | Safety Function Map |
| 2 | Lab 2 – IEC 62443 Mini Workshop | Zone / Conduit Diagram |
| 3 | Lab 3 – Threat & Risk | Risk Register |
| 4 | Lab 4 – Secure Remote Access | Secure Architecture |

Detaylı makine analizi, SWOT ve gereksinim analizi: [`Ceotherm_Homojenizasyon_Analiz.docx`](./Ceotherm_Homojenizasyon_Analiz.docx)

## Kaynaklar
- [CEOTHERM – Homojenizasyon Tesisleri (TR)](https://ceotherm.com.tr/homojenizasyon-tesisleri/)
- [CEOTHERM – Homogenization Facilities (EN)](https://ceotherm.com/homogenization-facilities/)

*Bu bir eğitim çalışmasıdır. Emniyet mimarisi ve ağ yapısıyla ilgili bazı kısımlar üreticinin sitesinde yer almadığı için varsayımdır.*
