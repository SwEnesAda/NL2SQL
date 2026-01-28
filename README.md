# 🔔 n8n GitHub Issue Takip Otomasyonu

Bu proje, **n8n** kullanılarak oluşturulmuş basit bir **GitHub Issue takip otomasyonudur**.  
Amaç, belirli bir GitHub reposundaki issue’ları otomatik olarak kontrol etmek ve gerekli durumlarda issue’lara yorum eklemektir.

---

## 🚀 Ne yapar?

- Belirtilen GitHub reposunu belirli aralıklarla kontrol eder  
- Repo içinde **issue (sorun)** olup olmadığını tespit eder  
- Issue varsa, ilgili issue’ya **otomatik olarak yorum ekler**

---

## 🧠 Nasıl Çalışır?

Workflow aşağıdaki adımlardan oluşur:

1. **Schedule Trigger** ile workflow belirli aralıklarla çalışır  
2. **HTTP Request (GitHub API)** ile repository issue’ları çekilir  
3. Gelen veri **Set node** ile sadeleştirilir  
4. **IF node** ile issue olup olmadığı kontrol edilir  
5. Issue varsa **otomatik yorum** eklenir  

---

## 🛠 Kullanılan Teknolojiler

- n8n  
- GitHub REST API  
- GitHub Personal Access Token  

---

## ⚙️ Nasıl Kullanılır?

1. Bu repoyu klonlayın veya indirin  
2. `github-issue-tracker-n8n.json` dosyasını **n8n** içerisine import edin  
3. GitHub üzerinden bir **Personal Access Token** oluşturun  
4. Token’ı **n8n Credentials** bölümüne ekleyin  
5. Repo owner ve repo adını kendinize göre düzenleyin  
6. Workflow’u **aktif** hale getirin  

---

## ⚠️ Not

Bu proje öğrenme ve otomasyon mantığını kavrama amacıyla hazırlanmıştır.  
Production ortamları için ek güvenlik ve hata yönetimi önerilir.
.
---

## 📄 Lisans

MIT License
