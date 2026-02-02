# n8n NL2SQL Otomasyonu

Bu proje, **n8n kullanılarak oluşturulmuş basit bir NL2SQL (Natural Language to SQL) otomasyonudur**.

## 🚀 Ne yapar?
- Kullanıcıdan doğal dilde sorgu alır
- Yapay zekâ ile sorguyu PostgreSQL SQL diline çevirir
- Sadece SELECT sorguları üretir
- Oluşturulan SQL sorgusunu PostgreSQL üzerinde çalıştırır
- Sorgu sonucunu kullanıcıya döndürür

## 🧠 Nasıl çalışır?
1. Chat Trigger ile workflow çalışır
2. AI Agent (LangChain) kullanıcı mesajını alır
3. Google Gemini Chat Model SQL üretir
4. AI Agent yalnızca PostgreSQL uyumlu SELECT sorgusu döndürür
5. Postgres Tool sorguyu veritabanında çalıştırır

## 🛠 Kullanılan Teknolojiler
- n8n
- LangChain
- Google Gemini (PaLM)
- PostgreSQL
- NL2SQL

## ⚙️ Nasıl kullanılır?
1. Bu repoyu klonlayın veya indirin
2. Workflow JSON dosyasını n8n’e import edin
3. Google Gemini (PaLM) API Key oluşturun
4. API Key’i n8n Credentials bölümüne ekleyin
5. PostgreSQL bilgilerinizi n8n Credentials’a tanımlayın
6. Workflow’u aktif hale getirin
7. Chat üzerinden doğal dilde sorgu gönderin

## 📁 Workflow Dosyası
workflow/nl2sql-n8n.json

Oluşturan: **SwEnesAda**
