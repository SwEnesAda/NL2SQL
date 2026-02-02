8n NL2SQL (Natural Language to SQL) Otomasyonu

Bu proje, n8n kullanılarak oluşturulmuş yapay zekâ destekli bir NL2SQL (Natural Language to SQL) otomasyonudur.

Kullanıcının doğal dilde yazdığı soruları alır, PostgreSQL uyumlu SELECT SQL sorgularına dönüştürür ve sonucu veritabanından otomatik olarak getirir.

🚀 Ne yapar?

Kullanıcıdan doğal dilde sorgu alır (chat üzerinden)

Yapay zekâ ile sorguyu PostgreSQL SQL diline çevirir

Sadece SELECT sorguları üretir

Oluşturulan SQL sorgusunu PostgreSQL üzerinde çalıştırır

Sonuçları kullanıcıya döner

🧠 Nasıl çalışır?

Chat Trigger ile kullanıcıdan mesaj alınır

AI Agent (LangChain), kullanıcı mesajını SQL’e çevirir

Google Gemini Chat Model, dil modeli olarak kullanılır

AI Agent sadece geçerli PostgreSQL SELECT sorgusu üretir

Üretilen sorgu Postgres Tool ile veritabanında çalıştırılır

🛠 Kullanılan Teknolojiler

n8n

LangChain (AI Agent)

Google Gemini (PaLM) Chat Model

PostgreSQL

NL2SQL yaklaşımı

⚙️ Nasıl kullanılır?

Bu repoyu klonlayın veya indirin

Workflow JSON dosyasını n8n’e import edin

Google Gemini (PaLM) API Key oluşturun

API Key’i n8n Credentials bölümüne ekleyin

PostgreSQL veritabanı bilgilerinizi n8n Credentials’a tanımlayın

Workflow’u aktif hale getirin

Chat üzerinden doğal dilde sorgu gönderin

📁 Workflow Dosyası

workflow/nl2sql-n8n.json

Oluşturan: SwEnesAda 🚀
