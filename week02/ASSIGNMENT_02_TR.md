# 2. Hafta Ödevi — Teklif Bölüm A + Gereksinimler

**Teslim:** Cumartesi 23:59 · Proje reponuza commit edin

> **Dersten önce** reponuzun kökündeki `AI_PLATFORMS_AND_STORES_TR.md` dosyasını okuyun —
> teknoloji seçimi bu hafta başlıyor.

Bu, ne yapacağınıza karar verdiğiniz hafta. On hafta onun üzerinde çalışacak, onu bir
mağazada yayınlayacak ve Aralık'ta savunacaksınız. Bu yüzden teklif bir formalite
değil. Bundan sonra denetleyicinin her hafta okuduğu ilk belge o.

---

## Bu haftayla gelenler

Bir şey yazmadan **önce** denetleyiciyi bir kez çalıştırın:

```bash
python .github/check_deliverables.py
```

Bu haftanın dosyalarını reponuza getirir: kökte `PROPOSAL.md`, `week02/` içinde `SRS.md`,
`requirements.json`, `contributors_02.json`, `ai_log_02.md` — artı kökte değişen ders
belgeleri. Hepsi iskelet. Yazmaya başlamadan içlerindeki yönergeleri okuyun: her bölüm
**ne** yazılacağını söylüyor ve bir **zayıf**, bir **güçlü** örnek gösteriyor. Örneklerin
hepsi uydurma tek bir projeyi anlatıyor ("StudyRoom", kütüphanede çalışma odası
rezervasyonu); böylece belgelerin birbirine nasıl bağlandığını görürsünüz. Sizin
projeniz değil ve kopyalanacak metin değil — kendi projenizi yazın. İskeletler
İngilizce; kendi metninizi Türkçe ya da İngilizce yazabilirsiniz. Doldurun; adlarını
değiştirmeyin. (Çevrimdışıysanız ya da çalışmazsa: `git fetch template && git checkout
template/main -- week02 PROPOSAL.md` aynı işi yapar, bkz. kurulum kartı.)

---

## Laboratuvarda — ders bitmeden push edilecek

### 1. `PROPOSAL.md` — Bölüm A, §1–§4

Başlık, tek paragraf özet, problem, çözüm. Her başlık ideal bir uzunluk veriyor; bu bir
sınır değil, yol gösterici — fikriniz gerektiriyorsa daha uzun yazın. Yorumlar GitHub'da görünmez ve sayılmaz; yazarken yerinde
bırakabilirsiniz. Önce §3'ü, sonra §4'ü yazın; §2 özeti ve §1 başlığı en sona bırakın —
ancak yazdığınızı özetleyebilirsiniz. Ders, denetleyicinin göremediği ama benim
gördüğüm iki şeyi gösterir: tek bir somut durum olarak yazılmış problem üç genel
iddiadan iyidir; neyi **yapmadığını** söyleyen çözüm, bitirilen çözümdür.

Ürünün üç zorunlu parçası var — **mobil uygulama, web istemcisi ve sunucu** — ve 11.
Hafta'ya kadar **public bir mağazada** yayınlanır. Kullanıcılar e-postayla gönderilen 4
haneli bir kodla giriş yapar; giriş her projede aynıdır. Önemsediğiniz ve on haftaya
sığan bir şey seçin. Küçük başlayın: 10. Hafta'da hala bir özellik ekleyebilirsiniz, ama
11. Hafta'da bir özelliği çıkarmak için çok geçtir.

### 2. Sınıf arkadaşlarınıza anlatın (isteğe bağlı) — `week02/contributors_02.json`

Salondaki en çok iki kişiye ne yapacağınızı §1–§4'ten, iki dakikada anlatabilirsiniz. Bu adım
isteğe bağlıdır. Onlar ilk
**paydaşlarınız**: ne işe yaradığını, neyi yapmadığını, ondan ne beklediklerini sorarlar.
Öğrenci numaralarını `week02/contributors_02.json` içine `stakeholder` rolüyle ve **her
biri için gerçekten ne söylediğini anlatan bir cümleyle** yazın — sordukları bir soru,
istedikleri bir özellik, bir itiraz. Arkasında hiçbir şey olmayan iki numara liste
demektir, kanıt değil; ne size insan katkısı puanını ne de onlara bonusu kazandırır.

Gelecek hafta adını yazacağınız kişilerden farklı olmalılar.

### 3. `week02/requirements.json` — ilk liste

En az **8 gereksinim**: en az **5 işlevsel** (sistem ne yapar — "öğrenci boş bir
aralığı rezerve eder") ve en az **3 işlevsel olmayan** (ne kadar iyi — hız, güvenlik,
gizlilik, kapasite; her zaman bir sayıyla). Her birinin bir kimliği `REQ-001`,
`REQ-002` …, test edilebilir tek bir davranışı anlatan bir `description`'ı ve
`functional: true/false` değeri var. İskeletin en üstündeki blok her alanı açıklıyor.

İkisi iskelette dolu geliyor: **REQ-001, e-postayla gönderilen 4 haneli kodla giriş** ve
**REQ-006, telefon ekranında kullanılabilir olmak**. REQ-001 ve REQ-006 herkes için
aynıdır; ifadeyi ürününüze göre uyarlayın. Gereksinim kimlikleri bu haftadan sonra hiç
değişmez. Sonraki işler bir zincirle onları gösterir: gereksinim → use case → ekran →
test case → api.md satırı. Sonradan vazgeçtiğiniz bir gereksinim kimliğini korur ve
`"dropped": true` alır.

Derste açıklamalar yeterli. Cumartesiye kadar her gereksinime iki alan daha eklenir:

- `priority` — `must` (o olmadan ürünün anlamı yok), `should` (önemli, yalnızca zaman
  biterse kesilir) ya da `could` (olsa iyi olur). Her şey must değildir: neyin
  kesilebileceğine karar vermek bu alanın amacı; hepsi must olan liste denetleyiciden geçmez.
- `acceptance` — gereksinimin karşılandığını kanıtlayan test: ne yaparsınız ve ne
  görmeniz gerekir. *"E-postadaki kodu 10 dakika içinde gir: giriş yapılır. Üst üste üç
  yanlış kod: 15 dakika kilit."* 4. haftadan itibaren gerçekten çalıştıracağınız bir test
  case'e dönüşür; çalıştırabileceğiniz bir test yazın.

### 4. Push

```bash
python .github/check_deliverables.py
git add .
git commit -m "week02: proposal part A, stakeholders, first requirements"
git push
```

Derste çalışmanızı 10:00, 11:00 ve 11:45 civarında (her saatten en fazla 15 dakika önce
ya da sonra) push edin; her push'ta yeni iş olsun. Ders notu, dersin sonuna dek push ettiğiniz son commit'i okur.
Push edilmemiş olan yoktur.

---

## Cumartesi 23:59'a kadar

### 5. `PROPOSAL.md` — §5–§7

**§5 Nasıl çalışır**: üç parçayı — mobil, web, sunucu — adlandırmalı, verinin nerede
durduğunu ve girişin nasıl olduğunu söylemeli ve başlığın hemen altında Mermaid ile bir
**sistem bağlam diyagramı** taşımalı: sisteminiz tek kutu, çevresinde her aktör ve dış
servis. **§6 Teknolojiler**: katman başına bir satır, yalnızca bu dönem kuracaklarınız
(`AI_PLATFORMS_AND_STORES_TR.md`, bilgisayarınızın ve telefonunuzun neye izin verdiğini söylüyor).
Web satırı herkes için aynıdır: `web/` klasöründeki düz HTML, CSS ve JavaScript sayfaları;
onları FastAPI sunucunuz sunar. Yalnızca mobil çatı sizin seçiminizdir. **§7 Başarı
ölçütleri**: Aralık'ta birinin ölçebileceği üç–beş ifade; her biri bir kullanıcı, bir
eylem ve bir sayı içerir. "Çalışıyor" bunlardan biri değildir.

Ayrıca `requirements.json` içinde her gereksinime bir `priority` ve bir `acceptance`
testi (bkz. 3. adım).

### 6. `week02/SRS.md`

SRS, insanların ürününüzü nasıl kullandığını anlatır: amaç ve kapsam, aktörler, en az
**üç kullanım senaryosu** (neyin ters gidebileceğiyle birlikte), kullanım senaryosu
başlığının altında Mermaid ile bir **kullanım senaryosu diyagramı** ve kısıtlarınız.
Bir–iki sayfa, otuz değil.

Gereksinimlerin tek yeri `week02/requirements.json` dosyasıdır. Onları SRS'e
kopyalamayın. SRS §4 ve §5'te tek satır durur: "The requirements are in
`week02/requirements.json`." İskelette bu satır zaten var.

Her kullanım senaryosunu iskeletin gösterdiği biçimde yazın: bir ad, aktör, kapsadığı
gereksinimler, üç–altı numaralı adımda **ana akış** ve **ne ters gidebilir**. Son kısım
genelde atlanır; eksik gereksinimleri bulduran da odur.

### 7. Taslak için yapay zeka kullanın — sonra yanlışını yakalayın — `week02/ai_log_02.md`

İki farklı asistandan, §1–§4'ünüze dayanarak *sizin* projeniz için öncelikleri ve kabul
ölçütleriyle sekiz gereksinim isteyin. İkisine aynı istemi verin (iskelet bir istem
öneriyor). Bu, haftanın tekniğidir (AI_Doc5 §4, çapraz sorgu). Emin görünen ama ürününüz için yanlış
gereksinimler üretecekler — uydurma özellikler, elinizde olmayan veriler, §4'ünüzle
çelişen kısıtlar. **Böyle bir hatayı belgeleyin**, yazışmayı Evidence bloğuna yapıştırın,
nasıl fark ettiğinizi ve neyi değiştirdiğinizi söyleyin. Yapay zekanın yardımcı olduğunu
söyleyip başka bir şey söylemeyen günlük hiçbir şey kazandırmaz; boş Evidence bloğu da.

### 8. Yeniden push, kontroller yeşil

```bash
python .github/check_deliverables.py
git add .
git commit -m "week02: proposal part A complete, SRS, requirements"
git push
```

Ders dışındaki commit kuralı:

- Yeni iş içeren en az iki commit, aralarında en az bir saat olacak şekilde push edilmiş
  olsun. Mesajlar ne değiştiğini söylesin.
- Commit'in üzerindeki tarih değil, GitHub'ın push saati sayılır.
- Bir kodlama ajanının yaptığı commit hiçbir zaman sayılmaz.
- **Asla force push yapmayın** ve bir asistanın yapmasına da izin vermeyin.

---

## Teslim listesi

**Laboratuvarda**
- [ ] `PROPOSAL.md` §1–§4 dolu, başlıklar değişmemiş
- [ ] `week02/contributors_02.json` — en çok iki paydaş (isteğe bağlı), numaraları ve her biri için bir cümle
- [ ] `week02/requirements.json` — ≥8 kayıt, `REQ-NNN` kimlikleri, ≥5 işlevsel, ≥3 işlevsel olmayan

**Cumartesi'ye kadar**
- [ ] `PROPOSAL.md` §5–§7 dolu; §5 mobil, web ve sunucuyu adlandırıyor ve Mermaid diyagramı var
- [ ] `week02/requirements.json` — her gereksinimde `priority` (hepsi `must` değil) ve `acceptance` testi
- [ ] `week02/SRS.md` — aktörler, ana akışı ve ne ters gidebileceğiyle ≥3 kullanım senaryosu, kullanım senaryosu diyagramı; §4 ve §5 `requirements.json` dosyasını gösteriyor (gereksinimlerin kopyası yok)
- [ ] `week02/ai_log_02.md` — belgelenmiş bir yapay zeka hatası, yapıştırılmış Evidence bloğu, nasıl fark ettiğiniz
- [ ] Kontroller GitHub'da yeşil; 1. Hafta hala geçiyor
- [ ] Derste 10:00, 11:00 ve 11:45 civarında push; ders dışında aralarında en az bir saat olan en az iki commit push edilmiş

---

## Bu hafta değil

Kod yok, API anahtarı yok. Teklifin B Bölümü — pazar, rakipler, ticari potansiyel,
teknik riskler ve **seçtiğiniz mağaza** — gelecek hafta. Tasarım 5. Hafta'da gelir. B
Bölümünü şimdi yazmayın: gelecek haftaki inceleme fikrinizi değiştirecek, değişiklik
günlüğü tam da bunun için var.

---

## Bu hafta nasıl notlanıyor

**Ders sonu — 5 puan.** §1–§4, varsa paydaşlar, ilk gereksinim listesi — ders bittiği anda
reponuzdan okunur ve sınıf panosunda gösterilir.

**Cumartesi 23:59 — 5 puan.** Son durumda kontroller yeşil: **2**. İnsan katkısı: **2**
— kanıtıyla kendi `ai_log_02.md` dosyanız ve paydaş yazdıysanız her ismin arkasında gerçek
bir cümle. Commit disiplini: **1** — dersteki push'lar (4. adım) ve 8. adımdaki kural.

**Katkı bonusu.** Adını yazdığınız her paydaş sizin haftalık notunuzun %10'unu
kazanır; dinlediğiniz sunumlar için siz de aynısını kazanırsınız. Bu hafta: en fazla iki.

Bir LLM bu teklifin her bölümünü yazabilir. Yapamadığı, hangi cümlelerinin sizin
fikriniz hakkında yanlış olduğunu bilmek ya da teklifi 5. Hafta'da yazacağınız
tasarımla uyumlu kılmaktır. Değerlendirilen budur.
