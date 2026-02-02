n8n NL2SQL Otomasyonu

Bu proje, n8n kullanılarak oluşturulmuş basit bir NL2SQL (Natural Language to SQL) otomasyonudur.

Kullanıcının doğal dilde yazdığı soruları alır ve PostgreSQL uyumlu SELECT SQL sorgularına dönüştürerek veritabanı üzerinden çalıştırır.

🚀 Ne yapar?

Kullanıcıdan chat üzerinden doğal dilde sorgu alır

Yapay zekâ ile sorguyu PostgreSQL SQL diline çevirir

Sadece SELECT sorguları üretir

Oluşturulan SQL sorgusunu PostgreSQL üzerinde çalıştırır

Sorgu sonucunu kullanıcıya döndürür

🧠 Nasıl çalışır?

Chat Trigger ile kullanıcı mesajı alınır

AI Agent (LangChain) kullanıcı mesajını analiz eder

Google Gemini Chat Model SQL üretimi için kullanılır

AI Agent yalnızca geçerli PostgreSQL SELECT sorgusu döndürür

Üretilen sorgu Postgres Tool ile çalıştırılır

🛠 Kullanılan Teknolojiler

n8n

LangChain AI Agent

Google Gemini (PaLM) Chat Model

PostgreSQL

NL2SQL yaklaşımı

⚙️ Nasıl kullanılır?

Bu repoyu klonlayın veya indirin

Workflow JSON dosyasını n8n’e import edin

Google Gemini (PaLM) API Key oluşturun

API Key’i n8n Credentials bölümüne ekleyin

PostgreSQL bağlantı bilgilerini n8n Credentials’a tanımlayın

Workflow’u aktif hale getirin

Chat üzerinden doğal dilde SQL sorgusu gönderin

📁 Workflow Dosyası

workflow/nl2sql-n8n.json

Oluşturan: SwEnesAda
