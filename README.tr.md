# LinqCheck GEO Skill

**E-ticaret için kanıta dayalı GEO ve AI Commerce hazırlık denetimi.**

[English README](README.md) · [Metodoloji](references/methodology.md) · [Kontrol listesi](references/checklist.md) · [Örnek](examples/sample-audit.md) · [Testler](TESTS.md)

Sürüm **0.1.1 — deneysel herkese açık beta**. TalyNext tarafından geliştirilir.

## Ne yapar?

Herkese açık ürün sayfalarında kimlik, varyant, fiyat, stok, kategori bilgisi, yapılandırılmış veri ve teknik erişim kontrollerini mevcut kanıtlarla değerlendirir. Ölçülen, gözlemlenen, çıkarılan ve doğrulanamayan bilgileri ayırır. Türkçe ve İngilizce raporlarda öncelikli aksiyonlar ve yeniden test kriterleri sunar.

Genel GEO puanı, görünürlük garantisi, otomatik site değişikliği veya satın alma sunmaz. Bağımsız bir tarayıcı değil, ajan talimatları paketidir; sonuçlar istemcinin modeline, araçlarına ve erişim koşullarına bağlıdır.

## Kurulum

Depoyu `linqcheck-geo-skill` adlı klasöre indirin veya klonlayın. Uyumlu Agent Skills istemcinizin kurulum yöntemini kullanın. Claude Code için proje içinde `.claude/skills/linqcheck-geo-skill/` veya kişisel kullanımda `~/.claude/skills/linqcheck-geo-skill/` klasörüne yerleştirin. ZIP kabul eden istemcilerde ilgili kurulum talimatını izleyin.

Örnek: “LinqCheck GEO Skill kullanarak https://example.com/product adresini GEO ve AI Commerce hazırlığı açısından analiz et. Kanıtları, kapsamı ve öncelikli aksiyonları göster. Salt okunur çalış.”

## Test durumu

Önceki sürümde 13 keşif amaçlı test faaliyeti yapıldı; tüm kabul kriterleri geçilmedi. v0.1.1 için Dagi, Seda Yalçın Atelier ve Allbirds ajan testleri 24 Kasım 2026 tarihinde incelendi ve çekincelerle deneysel beta için kabul edildi. Tam regresyon ve bağımsız doğrulama henüz tamamlanmadı. Bağımsız doğruluk veya standart ajana üstünlük iddiası yoktur. Ayrıntılar: [TESTS.md](TESTS.md).

## Ticari şeffaflık ve lisans

TalyNext aynı zamanda [LinqCheck](https://linqcheck.com) ticari ürününü geliştirir. Skill kullanımı için üyelik, ödeme veya zorunlu LinqCheck çağrısı gerekmez. Kullanılan istemci ve araçların kendi veri işleme koşulları geçerlidir. Skill telemetri kodu içermez.

Hata bildirimlerinde kişisel bilgileri ve kimlik bilgilerini paylaşmayın. Lisans: [LinqCheck Community License — Version 1.0](LICENSE). Bireysel kullanım, eğitim, araştırma ve şirketin kendi iç ticari operasyonları için ücretsiz kullanıma izin verilir. Ticari faaliyet kapsamında üçüncü taraflara sunulan analiz ve danışmanlık (ücretsiz tanıtım analizleri dahil), üçüncü taraflara sunulan ticari entegrasyonlar, yeniden satış ve herkese açık yeniden dağıtım için lisans, GitHub kullanım koşulları ve uygulanabilir hukuk çerçevesinde ayrı yazılı izin gerekir. Ticari izin talepleri: [LinqCheck](https://linqcheck.com). Kaynak erişilebilir (source-available); OSI onaylı açık kaynak değildir. İngilizce lisans metni esastır.
