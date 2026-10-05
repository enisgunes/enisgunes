<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:4F46E5,100:06B6D4&height=240&section=header&text=Merhaba,%20ben%20Enis%20👋&fontSize=48&fontColor=ffffff&animation=fadeIn&fontAlignY=34&desc=.NET%20%7C%20React%20%7C%20Kurumsal%20Entegrasyonlar%20%7C%20Multi-Tenant%20SaaS&descAlignY=52&descSize=18" width="100%"/>

<p align="center" style="font-size:17px">
ERP ve e-İrsaliye/e-Fatura entegrasyonları geliştiriyorum ·<br/>
çoklu kiracılı (multi-tenant) SaaS platformları kuruyorum ·<br/>
arka planda sessizce çalışan, güvenilir sistemler yazıyorum
</p>

<br/>

<a href="https://www.linkedin.com/in/enisguness" target="_blank">
  <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" />
</a>
<a href="https://github.com/enisgunes" target="_blank">
  <img src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
</a>
<a href="mailto:enis.gunes@saldos.com.tr">
  <img src="https://img.shields.io/badge/E--posta-EA4335?style=for-the-badge&logo=gmail&logoColor=white" />
</a>

<br/><br/>

<img src="https://img.shields.io/badge/.NET-512BD4?style=for-the-badge&logo=dotnet&logoColor=white" />
<img src="https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white" />
<img src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
<img src="https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white" />
<img src="https://img.shields.io/badge/SQL_Server-CC2927?style=for-the-badge&logo=microsoftsqlserver&logoColor=white" />
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" />

</div>

<br/>

## 🧭 Ne İş Yapıyorum

Perakende, kozmetik ve sağlık sektöründeki şirketler için **ERP entegrasyonları**, **e-fatura/e-irsaliye** süreçleri ve **çok kiracılı (multi-tenant) web platformları** geliştiriyorum. İşimin büyük bölümü ekranda görünmeyen, arka planda 7/24 sessizce çalışan, hata toleransı düşük sistemler: muhasebe/ERP veritabanlarıyla veri senkronizasyonu, devlet entegrasyonları (GİB) ve uçtan uca dijitalleştirilmiş iş süreçleri.

<table>
<tr>
<td width="50%" valign="top">

**🏗️ Mimari & Backend**
- Clean Architecture, CQRS (MediatR), FluentValidation
- Repository / Unit of Work, event-driven servisler
- RabbitMQ / MassTransit ile mesajlaşma, Saga/State Machine akışları
- Arka plan servisleri: Windows Service / `BackgroundService`, zamanlanmış işler

</td>
<td width="50%" valign="top">

**🔌 Entegrasyon & Veri**
- SOAP/REST tabanlı ERP entegrasyonları (LOGO/Netsis tarzı şemalar)
- GİB e-İrsaliye / e-Fatura (UBL-TR) üretimi ve özel entegratör (SOAP) gönderimi
- Multi-tenant izolasyon: tenant başına veritabanı/şema, dinamik tenant çözümleme
- Webhook, SMS/WhatsApp/e-posta bildirim altyapıları

</td>
</tr>
</table>

---

## 🛠️ Teknoloji Yığını

<div align="center">
<img src="https://skillicons.dev/icons?i=cs,dotnet,react,ts,js,nextjs,tailwind,mssql,redis,docker,git,nodejs,py,fastapi&theme=dark" />
</div>

<br/>

| Katman | Teknolojiler |
|---|---|
| **Backend** | C#, .NET 8 / 9 / 10, ASP.NET Core Web API, Entity Framework Core, Dapper, MediatR, FluentValidation, SignalR, Hangfire |
| **Frontend** | React, TypeScript, Vite, Next.js, Tailwind CSS, shadcn/ui, TanStack Query |
| **Veri & Mesajlaşma** | SQL Server, Redis, RabbitMQ / MassTransit |
| **Altyapı & Araçlar** | Docker, IIS, Windows Services, Serilog, JWT / Role-based Auth |
| **Diğer** | Python (FastAPI), REST/SOAP entegrasyonları, Node.js |

---

## 💼 Öne Çıkan Çalışma Alanları

<details open>
<summary><b>🧾 E-İrsaliye / E-Fatura Entegrasyonları</b></summary>
<br/>

ERP veritabanlarından sevkiyat verisini okuyup GİB'in **UBL-TR DespatchAdvice** formatına çeviren ve özel entegratör (ICE Teknoloji) SOAP servisleri üzerinden GİB'e gönderen `.NET Worker Service`'ler.

- Şema kurallarının (eleman sırası, VKN/TCKN ayrımı, muhtelif müşteri senaryosu) deneme-yanılmayla keşfedilip dokümante edildiği, üretime hazır entegrasyon katmanları
- Kargo firması ZPL etiketlerine e-irsaliye QR kodunu basım anında enjekte eden, çok kiracılı ayrı bir dönüştürme servisi (her kargo firması + müşteri kombinasyonu için özelleştirilmiş etiket yerleşimi)
- Idempotent işleme, kapsamlı Serilog + MSSQL loglama, tenant başına izole hata yönetimi

</details>

<details>
<summary><b>🏬 Multi-Tenant İşletme Yönetim Platformu</b></summary>
<br/>

Servis/bakım sektörü için; müşteri, araç, iş emri, randevu, stok, ön muhasebe ve raporlama modüllerini tek bir sistemde birleştiren SaaS uygulaması.

- Tenant başına izole veritabanı (DB-per-tenant), subdomain/özel alan adı bazlı otomatik tenant çözümleme
- Granüler izin sistemi, durum makineleriyle yönetilen iş emri/teklif akışları
- **App Market** modeli: özellikler bağımsız modüller olarak ayrı ayrı satın alınabilir
- Müşteri self-servis akışları (login'siz randevu, teklif onayı, canlı takip, memnuniyet anketi)

</details>

<details>
<summary><b>🛒 E-Ticaret & Satınalma Sistemleri</b></summary>
<br/>

Çok kiracılı e-ticaret altyapısı (katalog/varyant yönetimi, sipariş yaşam döngüsü, ödeme, kargo, B2B cari hesap, çoklu fiyat listesi) ve kurum içi satınalma onay süreçlerini uçtan uca yöneten web uygulamaları.

- Event-driven mimari (Outbox pattern, MassTransit/RabbitMQ), arama senkronizasyonu (Elasticsearch)
- Rol bazlı çok aşamalı onay akışları (personel → yönetici → onaylayıcı → admin)

</details>

<details>
<summary><b>📊 Raporlama & İzleme Servisleri</b></summary>
<br/>

- Birden fazla ERP/veritabanından veri derleyip çok sekmeli, performans odaklı Excel raporları üreten portallar
- Veritabanı sağlık kontrolü yapan, eşik aşımında alert/webhook (Slack/Teams) gönderen izleme aracı
- Kritik Windows servislerinin ayakta kalıp kalmadığını izleyen, kesinti durumunda e-posta uyarısı gönderen bir gözlemci servis

</details>

<details>
<summary><b>💬 WhatsApp/SMS Bildirim Otomasyonu</b></summary>
<br/>

Kuyruk tabanlı, insan davranışını taklit eden (random gecikme, typing simülasyonu, günlük/saatlik limitler, çalışma saatleri) bir WhatsApp gönderim ve hatırlatma servisi; randevu/iş emri/teklif süreçlerine bağlı otomatik müşteri bildirimleri.

</details>

<details>
<summary><b>🔐 Güvenlik & Erişim Araçları</b></summary>
<br/>

- Kurumsal şifre yönetimi: AES-256 şifreleme + e-posta üzerinden gelen 2FA kodlarının SignalR ile gerçek zamanlı panele yansıtılması
- Yetki bazlı, çift yazma (dual-write) yedeklemeli kurumsal dosya paylaşım sistemi

</details>

---

## 📌 Notlar

Çalışmalarımın büyük kısmı müşteri verisi ve kurumsal sistemlerle doğrudan entegre olduğundan ilgili depolar **özel (private)** tutulmaktadır. Bu profil, geliştirdiğim sistemlerin kapsamını ve kullandığım teknolojileri özetlemek için hazırlanmıştır.

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:06B6D4,100:4F46E5&height=120&section=footer" width="100%"/>
</div>
