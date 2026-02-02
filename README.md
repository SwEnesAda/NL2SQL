# 🧠 n8n NL2SQL (Natural Language to SQL) Uygulaması

Bu proje, **n8n** ve **LLM (Google Gemini)** kullanılarak geliştirilmiş basit bir **NL2SQL (Doğal Dil → SQL)** uygulamasıdır.  
Amaç, kullanıcının doğal dilde sorduğu soruları **geçerli ve güvenli PostgreSQL SELECT sorgularına** dönüştürmek ve sonucu veritabanından almaktır.

---

## 🚀 Ne yapar?

- Kullanıcıdan **doğal dilde** bir soru alır  
- Soruyu **PostgreSQL uyumlu SELECT SQL sorgusuna** çevirir  
- Üretilen SQL sorgusunu PostgreSQL üzerinde çalıştırır  
- Sorgu sonucunu kullanıcıya döndürür  

Örnek:

```sql
SELECT COUNT(*) 
FROM users 
WHERE created_at >= NOW() - INTERVAL '30 days';
🧠 Nasıl Çalışır?

Workflow aşağıdaki adımlardan oluşur:

Chat Trigger
Kullanıcıdan doğal dilde mesaj alır

AI Agent (LangChain)
Doğal dili SQL’e çeviren ana bileşendir

Sadece SQL üretir

Markdown veya açıklama döndürmez

Yalnızca SELECT sorgularına izin verir

PostgreSQL uyumludur

Google Gemini Chat Model

LLM olarak kullanılır

temperature = 0 ile deterministik sonuçlar üretir

PostgreSQL Tool

Üretilen SQL sorgusunu PostgreSQL veritabanında çalıştırır

Sonucu workflow çıktısı olarak döndürür
🛠 Kullanılan Teknolojiler

n8n

LangChain (n8n Agent Node)

Google Gemini (PaLM) API

PostgreSQL

NL2SQL (Natural Language to SQL)

⚙️ Nasıl Kullanılır?

Bu repoyu klonlayın veya indirin

Workflow JSON dosyasını n8n içerisine import edin

Google Gemini (PaLM) API Key oluşturun

API Key’i n8n Credentials bölümüne ekleyin

PostgreSQL bağlantı bilgilerinizi Postgres Credentials olarak tanımlayın

Veritabanı şemanızın sorgulara uygun olduğundan emin olun

Workflow’u aktif hale getirin

Chat üzerinden doğal dilde sorular sormaya başlayın

⚠️ Notlar

Güvenlik amacıyla yalnızca SELECT sorgularına izin verilmektedir

INSERT, UPDATE, DELETE gibi işlemler bilinçli olarak engellenmiştir

Production ortamları için:

Query validation

Schema bazlı yetkilendirme

Rate limiting

Logging & monitoring

eklenmesi önerilir.

📌 Kullanım Senaryoları

Teknik olmayan kullanıcılar için veri sorgulama

Chat tabanlı veri keşfi

BI / dashboard öncesi hızlı analiz

Internal tool ve prototip geliştirme

📄 Lisans

MIT License
