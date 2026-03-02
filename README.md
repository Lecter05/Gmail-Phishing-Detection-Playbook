

Videoda, gelen maildeki zararlı eki ve url'i kontrol ediyor. Ek henüz hiç taranmadığı için başta sonuç vermiyor, tarama işlemi tamamlandığında mail Trash'e taşınıyor.
Video playbookun nasıl çalıştığına dair fikir edinilmesi için kaydedildi. 

https://github.com/user-attachments/assets/e1d42c33-b949-43dc-b099-5739d7da9175



🔍 Ne yapıyor
* Gönderici IP'yi VirusTotal'de analiz ediyor
* Email içindeki URL'leri tespit edip VirusTotal'de tarıyor
* Email eklerini hash kontrolü + gerekirse VirusTotal'de analiz ediyor
* Blacklist/Whitelist kontrolü yapıyor
* Zararlı tespit edilirse email otomatik çöpe taşınıyor

🚧 Eksik / Geliştirilecek
* SPF/DKIM/DMARC fail
* Display name spoof
* yeni domain

Kullanım
1. https://login.tines.com/ hesap aç
2. /personal/stories sekmesinden New ⌵ simgesi
3. Import story

📌 Not
* API ler Credentials kısmından verilebilir.
* Whitelist ve Blacklist Resources kısımları kullanılarak kurgulandı.
* **Google Workspace (OAuth 2.0):** Sistemin e-postaları okuyabilmesi ve silebilmesi için console.cloud.google.com üzerinden **Gmail API** alınmıştır.
