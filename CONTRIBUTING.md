# Katkı Rehberi

Köprü'ye katkı verdiğiniz için teşekkürler. Bu rehber tüm depolar için geçerlidir. Kurallar kısa, ama istisnasızdır.

## Dil

- **Türkçe:** dokümanlar, issue'lar, PR açıklamaları, tartışmalar.
- **İngilizce:** kod, değişken adları, commit mesajları, branch adları.

## Çalışma akışı

1. **Issue ile başlayın.** Her iş bir issue'dur. Issue yoksa açın, şablonu doldurun. Kendinize atayın (`Assignees`).
2. **Board'u güncelleyin.** Issue'yu proje board'unda `Yapılacak → Devam ediyor` sütununa taşıyın.
3. **Branch açın.** `main` üzerinden, şu formatla:
   ```
   <tür>/<issue-no>-<kısa-açıklama>
   örnek: docs/12-use-case-diagram
          feat/34-referrer-invite
          fix/41-otp-timeout
   ```
4. **Küçük commit'ler atın.** [Conventional Commits](https://www.conventionalcommits.org/tr/v1.0.0/) formatı:
   ```
   docs: add functional requirements draft
   feat(invite): send referrer invite email
   fix(auth): reject non-TR phone numbers
   ```
   Türler: `feat`, `fix`, `docs`, `refactor`, `test`, `chore`, `ci`, `style`, `perf`.
5. **PR açın.** PR başlığı da Conventional Commits formatında olmalıdır (CI kontrol eder). Açıklamaya `Closes #<issue-no>` yazın.
6. **İnceleme.** En az **1 onay** gerekir. Kendi PR'ınızı kendiniz onaylayamazsınız. Tüm yorumlar çözülmeden birleştirilmez.
7. **Birleştirme.** Yalnızca **squash merge**. Birleştirmeden sonra branch otomatik silinir.

## `main` dalı korumalıdır

- Doğrudan push **yapılamaz**.
- Force push ve dal silme **kapalıdır**.
- Tüm CI kontrolleri yeşil olmadan birleştirilmez.
- Geçmiş doğrusal tutulur (squash).

## Depoya girmeyecekler

- **Kişisel veri.** Gerçek isim, telefon, e-posta, CV, kişisel bilgi içeren ekran görüntüsü. Örnek veri her zaman sahte olmalıdır.
- **Sırlar.** API anahtarı, şifre, token, `.env` dosyası. Sırlar GitHub Secrets veya ortam değişkenlerinde durur.
- **Üretilmiş dosyalar.** Build çıktısı, `node_modules`, cache, AI aracı çıktıları (graph, index, log). 1 MB üstü dosyalar CI'da reddedilir.

Yanlışlıkla sır veya kişisel veri push ettiyseniz **hemen** bir yöneticiye haber verin. Sadece silmek yetmez; anahtar iptal edilmelidir.

## Kararlar

Önemli teknik ve ürün kararları `docs` deposunda `kararlar/` altında **ADR** (Architecture Decision Record) olarak yazılır. Bir karar WhatsApp'ta konuşulabilir, ama yazıya geçmeden geçerli sayılmaz.

## Yapay zekâ ile çalışma

AI araçları (Claude, Copilot, Cursor vb.) serbesttir. Ama:

- Ürettiğiniz içeriği **siz** anlamak ve savunmak zorundasınız.
- AI çıktısını incelemeden PR açmayın.
- AI aracının oluşturduğu yardımcı dosyaları (cache, index, graph) commit etmeyin.

## İletişim

- Günlük koordinasyon: WhatsApp grubu.
- Kalıcı her şey: GitHub (issue, PR, ADR).
- Hocalarımıza soru: önce ekip içinde netleştirin, sonra tek ve toplu soru olarak iletin.

## Davranış

Tüm katılımcılar [Davranış Kuralları](CODE_OF_CONDUCT.md)'na uyar.
