# Güvenlik Politikası / Security Policy

Köprü kişisel veri işleyen gönüllü bir projedir. Güvenlik araştırmacılarının bildirimlerini memnuniyetle karşılıyoruz.

*Köprü is a volunteer project that handles personal data. We welcome reports from security researchers. English reports are welcome.*

## Nasıl bildirilir? / How to report

**Herkese açık issue, PR veya tartışma açmayın.** / *Do not open public issues, PRs or discussions.*

1. İlgili deponun **Security → Report a vulnerability** sekmesini kullanın (GitHub özel güvenlik bildirimi). Bildirim yalnızca yöneticilere görünür.
   *Use the repository's **Security → Report a vulnerability** tab (GitHub private vulnerability reporting).*
   - Örnek / example: <https://github.com/kopru-agi/docs/security/advisories/new>
2. Hangi depo olduğundan emin değilseniz `docs` deposunu kullanın.
   *If unsure which repository, use `docs`.*

Bildiriminizde şunlar olsun / *Please include:*

- Etkilenen depo, sayfa veya uç nokta / *affected repo, page or endpoint*
- Tekrar üretme adımları ve PoC / *reproduction steps and PoC*
- Olası etki: hangi veri, kimin verisi / *impact: which data, whose data*
- Önerilen çözüm (varsa) / *suggested fix (optional)*

## Süreç / Timeline

| Adım / Step | Süre / Target |
|---|---|
| Alındı bildirimi / Acknowledgement | 3 iş günü / 3 business days |
| İlk değerlendirme / Triage | 7 gün / 7 days |
| Düzeltme / Fix (kritik / critical) | 14 gün / 14 days |
| Koordineli açıklama / Coordinated disclosure | Düzeltmeden sonra veya en geç 90 gün / after the fix, or 90 days at most |

Kişisel veri ihlali şüphesinde, KVKK Kurulu kararı gereği ihlal en geç **72 saat** içinde değerlendirilir.
*Suspected personal-data breaches are assessed within 72 hours, as the Turkish DPA (KVKK) requires.*

Onaylanan bildirimler için GitHub Security Advisory yayımlanır ve izin verirseniz adınız teşekkür bölümüne eklenir. Para ödülü (bug bounty) yoktur; proje gönüllüdür.
*Confirmed reports get a GitHub Security Advisory and, with your consent, credit. There is no monetary bounty; this is a volunteer project.*

## Kapsam / Scope

**Kapsamda / In scope**

- `kopru-agi` organizasyonundaki tüm depolar / *all repositories in the `kopru-agi` organization*
- Yayına alındığında Köprü web uygulaması ve API'si / *the Köprü web app and API, once deployed*

**Kapsam dışı / Out of scope**

- Hizmet engelleme (DoS/DDoS), hacim testi / *denial of service, load testing*
- Sosyal mühendislik, oltalama, fiziksel saldırı / *social engineering, phishing, physical attacks*
- Üçüncü taraf hizmetler (GitHub, Resend, hosting sağlayıcısı) / *third-party services*
- Etkisi gösterilmemiş otomatik tarayıcı çıktıları / *unverified automated scanner output*
- Eksik güvenlik başlıkları, tek başına etkisi olmayan bulgular / *missing headers or best-practice findings with no demonstrated impact*

## Güvenli liman / Safe harbor

Bu politikaya iyi niyetle uyan araştırmaya karşı hukuki işlem başlatmayız. Şartlar:

*We will not pursue legal action against good-faith research that follows this policy, provided you:*

- Yalnızca **kendi oluşturduğunuz test hesaplarını** kullanın. Başka kullanıcıların verisine erişmeyin, değiştirmeyin, silmeyin.
  *Use only test accounts you created. Do not access, modify or delete other users' data.*
- Yanlışlıkla kişisel veriye eriştiyseniz durun, veriyi saklamayın ve hemen bildirin.
  *If you reach personal data by accident, stop, do not keep it, and report immediately.*
- Gerçek kişilere davet, SMS veya e-posta göndermeyin.
  *Do not send invites, SMS or email to real people.*
- Düzeltme yayımlanmadan bulguyu kamuya açıklamayın.
  *Do not disclose before a fix is released.*

## Desteklenen sürümler / Supported versions

Proje henüz geliştirme aşamasındadır. Yalnızca `main` dalı desteklenir.
*The project is pre-release. Only the `main` branch is supported.*
