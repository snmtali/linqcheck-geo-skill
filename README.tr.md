# LinqCheck GEO Skill

**E-ticaret için kanıta dayalı GEO ve AI Commerce hazırlık denetimi.**

[English README](README.md) · [Metodoloji](references/methodology.md) · [Kontrol listesi](references/checklist.md) · [Örnek](examples/sample-audit.md) · [Testler](TESTS.md)

Sürüm **0.1.2 — deneysel public beta**. Yayına hazırlandı; bağlantılar ilgili GitHub yayını ve dosyaları yayımlandığında çalışacaktır. TalyNext tarafından geliştirilir.

## Ne yapar?

Herkese açık ürün sayfalarında kimlik, varyant, fiyat, stok, kategori bilgisi, yapılandırılmış veri ve teknik erişim kontrollerini mevcut kanıtlarla değerlendirir. Ölçülen, gözlemlenen, çıkarılan ve doğrulanamayan bilgileri ayırır. Türkçe ve İngilizce raporlarda öncelikli aksiyonlar ve yeniden test kriterleri sunar.

Genel GEO puanı, görünürlük garantisi, otomatik site değişikliği veya satın alma sunmaz. Bağımsız bir tarayıcı değil, ajan talimatları paketidir; sonuçlar istemcinin modeline, araçlarına ve erişim koşullarına bağlıdır.

## Kurulum

[![GEO Skill İndir](https://img.shields.io/badge/Ücretsiz%20İndir-GEO%20Skill%20v0.1.2-00897B?style=for-the-badge)](https://github.com/snmtali/linqcheck-geo-skill/releases/download/v0.1.2/linqcheck-geo-skill-v0.1.2-community.zip)

**Bireysel ve şirket içi kullanım için ücretsiz.**

[Sürüm notlarını inceleyin](https://github.com/snmtali/linqcheck-geo-skill/releases/tag/v0.1.2)

Depoyu `linqcheck-geo-skill` adlı klasöre indirin veya klonlayın. Uyumlu Agent Skills istemcinizin kurulum yöntemini kullanın. Claude Code için proje içinde `.claude/skills/linqcheck-geo-skill/` veya kişisel kullanımda `~/.claude/skills/linqcheck-geo-skill/` klasörüne yerleştirin. ZIP kabul eden istemcilerde ilgili kurulum talimatını izleyin.

Örnek: “LinqCheck GEO Skill kullanarak https://example.com/product adresini GEO ve AI Commerce hazırlığı açısından analiz et. Kanıtları, kapsamı ve öncelikli aksiyonları göster. Salt okunur çalış.”

Skills.sh kurulumu (önce kaynak kodu ve kurulum izinlerini inceleyin):

```sh
npx skills add snmtali/linqcheck-geo-skill --skill linqcheck-geo-skill
```

Bu komut sabit hash ile doğrulanmış yayın dosyasını değil, depo kaynağını izler.

## Test durumu

25 Kasım 2026 tarihli rc.2 raporunda haricen hazırlanmış çevrimdışı girdilerde altı koşullu güvenlik geçişi, 14 uyumlu ve bir koşullu uyumlu metodoloji kriteri bildirildi. Nihai pakette yalnızca sürüm etiketleri ve belgeler değişti; nihai sürüm etkinleştirme ve davranış testleri tekrarlanmadı. Bağımsız araç/ağ kayıtları doğrulanmadı; W012 açıktır. Bkz. [SECURITY.md](SECURITY.md).

Önceki sürümde 13 keşif amaçlı test faaliyeti yapıldı; tüm kabul kriterleri geçilmedi. v0.1.1 için Dagi, Seda Yalçın Atelier ve Allbirds ajan testleri 24 Kasım 2026 tarihinde incelendi ve çekincelerle deneysel beta için kabul edildi. Tam regresyon ve bağımsız doğrulama henüz tamamlanmadı. Bağımsız doğruluk veya standart ajana üstünlük iddiası yoktur. Ayrıntılar: [TESTS.md](TESTS.md).

## Ticari şeffaflık ve lisans

TalyNext aynı zamanda [LinqCheck](https://linqcheck.com) ticari ürününü geliştirir. Skill kullanımı için üyelik, ödeme veya zorunlu LinqCheck çağrısı gerekmez. Kullanılan istemci ve araçların kendi veri işleme koşulları geçerlidir. Skill telemetri kodu içermez.

Hata bildirimlerinde kişisel bilgileri ve kimlik bilgilerini paylaşmayın. Lisans: [LinqCheck Community License — Version 1.0](LICENSE). Bireysel kullanım, eğitim, araştırma ve şirketin kendi iç ticari operasyonları için ücretsiz kullanıma izin verilir. Ticari faaliyet kapsamında üçüncü taraflara sunulan analiz ve danışmanlık (ücretsiz tanıtım analizleri dahil), üçüncü taraflara sunulan ticari entegrasyonlar, yeniden satış ve herkese açık yeniden dağıtım için lisans, GitHub kullanım koşulları ve uygulanabilir hukuk çerçevesinde ayrı yazılı izin gerekir. Ticari izin talepleri: [LinqCheck](https://linqcheck.com). Kaynak erişilebilir (source-available); OSI onaylı açık kaynak değildir. İngilizce lisans metni esastır.

## Kurulum bütünlüğü

Kurulumdan önce resmî depoyu ve yayın dosyalarını inceleyin. İndirilen v0.1.2 ZIP dosyasının özetini ilgili SHA-256 yayın dosyasıyla karşılaştırın.

Windows PowerShell: `Get-FileHash -Algorithm SHA256 <indirilen-zip>`

macOS: `shasum -a 256 <indirilen-zip>`

Linux: `sha256sum <indirilen-zip>`

Yer tutucu yerine gerçek dosya yolunu (gerekirse tırnak içinde) yazın. Eşleşme yalnızca referans değere göre bütünlüğü doğrular; yayıncı kimliğini veya güvenliği garanti etmez. Bkz. [SECURITY.md](SECURITY.md).
