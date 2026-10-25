# AIASD · 3. Hafta — Sunum, Akran İncelemesi, Teklif Bölüm B

*Atlas Üniversitesi · 2026–27 Güz · Prof. Dr. Vedat Coşkun*
*Bu sayfadan sunulur. Bölüm bölüm kaydırın; her `---` bir slayttır.*

<!-- Hoca: tarayıcıyı %150 yakınlaştır. Süreler notlarda. Toplam ≈ 3 saat:
10 dk giriş · 50 dk inceleme turu · projeyi kesinleştirmeye en az 30 dk (başlık, §3–§4) · 20 dk ekranlar · 11:45'e kadar çalışma · not, dersin sonuna dek push edilen son commit'i okur. -->

---

## Bugün

1. Geçen hafta nasıl geçti
2. Dönem boyunca kalacak iki kural
3. **Bugün projeniz kesinleşiyor: başlığı ve içeriği**
4. Pitch nedir, neden yazdınız
5. İnceleme turu — dörtlü gruplar, ilk saat
6. Turdan sonra: üç değerlendiren, gözden geçirilmiş teklif, değişiklik günlüğü, ana akışın ekranları
7. Cumartesiye kadar: Bölüm B, mağaza, düşman gözüyle okutma
8. Hafta nasıl notlanıyor

---

## 2. hafta sayılarla

| | İngilizce | Türkçe |
|---|---|---|
| Kayıtlı | 78 | 33 |
| Derste push yapan | 62 | 26 |
| Ders slotu 5 / 5 | 42 | 21 |
| Cumartesi: tüm kontroller yeşil | 57 | 21 |

Notlar ve denetleyicinin yorumları pazar günü **kendi reponuzda bir issue** olarak geldi.
Notla ilgili sorular oraya, yorum olarak — e-postayla değil.

---

## Dönem boyunca kalacak iki kural

**1. Proje *sizin* bir sorununuzu çözer — kendinizin, üniversitedeki arkadaşlarınızın
ya da sosyal çevrenizin.**
"Öğrenciler X'te zorlanıyor" değil. En son ne zaman oldu — size ya da gözünüzün önünde:
tarih, yer, kim, onun yerine ne yaptı.

**2. Çevrenizdeki gerçek kişiler kullanabilir.**
Atlas'ta, ailenizde, bir kulüpte. Beşi test edecek: 9. haftada beta testi, 10. haftada
Kullanıcı Kabul Testi. Onları bugün adlandırıyorsunuz.

Son seferi ya da beş kişiyi söyleyemiyorsanız sorun slaytta değil projededir. **Projeyi bu
derste değiştirin:** dersin sonunda (11:45) kesinleşiyor.

---

## Bugün projeniz kesinleşiyor

**Dersin sonunda (11:45): başlığı ve içeriği.** Dönem sonuna kadar aynı başlık, aynı problem ve aynı ürün.

Ayrıntıları değişmeye devam edebilir: özellikler, gereksinimler, kapsam. Her değişiklik Değişiklik günlüğünde bir satır alır. Projenin kendisi değişemez.

**Bu, dönemin en önemli kararıdır. Ona zaman ayırın.** Projeyi inceleme turunda sınayın; sonra grubunuzun cevapları önünüzdeyken §1'i (başlık) ve §3–§4'ü (problem ve ürün) kesinleştirmek için en az yarım saat ayırın.

Bugünden sonra yalnızca teknik olarak imkansız çıkan bir proje değişebilir; o da ancak benim bir issue'da yazılı onayımla.

---

## Pitch nedir

Pitch, bir fikri, karar verecek birine kısa, sıralı ve somut biçimde anlatıp bir şey istemektir: para, zaman, bir evet.

- **Kısa**, çünkü dikkat kıt bir kaynaktır.
- **Sıralı**: sorun → çözüm → kim → neden siz → ne istiyorsunuz.
- **Somut**: sayılar, isimler, bir örnek. Sıfat kanıt değildir.

> "Herkes için yenilikçi bir platform" pitch değildir.
> "Atlas kütüphanesinde her dönem 3.000 öğrenci oda arıyor; altıda biri odasız dönüyor;
> StudyRoom boş odayı gösterip 30 saniyede ayırtıyor" pitch'tir.

---

## Aynı şey, arkasında 2,5 milyon avroyla

**EIC Accelerator** — Avrupa Birliği'nin girişim hibesi (Horizon Europe).

Başvurunun 1. adımı tam olarak bu: **en fazla 10 slaytlık bir pitch deck**, **3 dakikalık
bir video**, kısa bir form. Yüzlerce başvuru bu üç şeyle elenir. On slayt: sorun · çözüm ·
neden şimdi · sayılarla pazar · rakipler ve farkınız · iş modeli · yol haritası ve riskler ·
ekip · istenen · sonraki adım.

Bugünkü altı slaydınız bu listenin ilk yarısı; cumartesi teslim edeceğiniz Bölüm B ikinci yarısı. Aralıktaki savunma ise küçük bir jüri önünde.

---

## Altı slaydınız — `week03/PITCH_03.md`

1. Ürün tek cümleyle
2. **Sorun en son ne zaman oldu — size ya da gözünüzün önünde**
3. **Onu test edecek beş kişi** (9.–10. haftalar) — ad, nereden tanıdığınız, neden
4. Üç gereksinim — *`requirements.json` ile aynı id ve aynı metin* — ve bir "yapmaz"
5. Ana ekran, **elle çizilmiş**
6. Emin olmadığınız tek şey

Yedinci slayt sabittir: değerlendirenlerinizin cevaplayacağı üç soru.

**Siz yazdınız, yapay zeka yok.** İçindeki her şey sizin hayatınız ve çevreniz. Herhangi
bir slaytı sorabilirim.

---

## Kendi bilgisayarınızdan sunmak

`week03/PITCH_03.md` dosyasını VS Code'da açın.

- **Marp for VS Code** eklentisiyle: önizleme düğmesi (sağ üst) slaytları gösterir; aynı
  düğme PDF ya da PPTX'e aktarır.
- Eklenti olmadan: VS Code'un normal Markdown önizlemesi (`⌘⇧V` / `Ctrl+Shift+V`) — slayt
  slayt kaydırın. Yeter.
- GitHub'ın web sitesinden değil: turdan sonra dosyayı düzenleyeceksiniz.

<!-- İkisini de test öğrencisinin PITCH_03.md'siyle projeksiyonda göster. 2 dk. -->

---

## İnceleme turu — dörtlü gruplar

**Dört kişilik grubunuzu şimdi kendiniz kurun.** Grup dönem boyunca sizinle kalacak; hangi haftalarda toplandığını ödevler söyler. Sınıf dörde bölünmediği için açıkta mı kaldınız? Bir gruba katılın; o grup beş kişi olur. Üç kişilik grup yok.

**Grubunuzu `week03/group_03.json` dosyasına yazın:** kendi numaranız dahil bütün üyelerin numaraları. Her üye aynı listeyi yazar. Listeler farklıysa grubun her üyesi bir puan kaybeder.

Herkes kendi bilgisayarından **5 dakika** sunar. Diğer üçü dinler; sonra üç sorunun her biri için birer cümle **yazar** ve sunana verir — kağıtta ya da bir metin dosyasında. Sonra sıradaki. Dört tur, yaklaşık **45 dakika**.

Değerlendirenler: ne düşünüyorsanız onu söyleyin. "İyi olmuş" kimseye yardım etmez, kimseye puan getirmez.

<!-- Grupları kurmaları için üç dakika verin; artanları gruplara yönlendirin. Dolaşın. 12 dakikada bir uyarın. -->

---

## Üç soru — 7. slayt

1. **Gerçek mi?** Bu sorunu kendisinin ve 3. slayttaki beş kişinin gerçekten yaşadığına sizi ikna etti mi?
2. **Burada kullanılabilir mi?** O beş kişi 9. haftada bunu gerçekten kullanabilir mi —
   onları ne durdurur?
3. **Fazla mı, az mı?** Hangi parça 11. haftaya yetişmez — ya da ürün tek ekrana mı inmiş?

Her birine bir cümle. Sunan kişi cümlelerinizi reposuna geçirir; yanlarına adınız yazılır ve bunlar size katkı bonusu kazandırır.

---

## Turdan sonra — dersin sonuna (11:45) kadar

**`week03/contributors_03.json`** — üç değerlendireniniz: `reviewer` rolü, öğrenci numaraları ve her birinin **yazdığı en yararlı cümle, alıntı olarak**. Sonra `accepted: true/false` ve `why`. Gerekçeyle reddetmek olur; arkasında hiçbir şey olmayan "dedi, değiştirdim" olmaz.

**`PROPOSAL.md`** — üç cevap önünüzdeyken §1–§7'yi gözden geçirin. Her değişiklik için dosyanın sonundaki Değişiklik günlüğüne **tarihli bir satır**:

`2026-10-07 — §4: grup sohbeti çıkarıldı; iki değerlendiren WhatsApp varken kimsenin kullanmayacağını söyledi.`

Teklif değişebilir. Sessizce değişemez. **§1'i (başlık) ve §3–§4'ü şimdi kesinleştirin: dersin sonunda (11:45) değişmez hale geliyorlar.**

---


## Ana akışınızın ekranları — `week03/screens_03.md`

Girişten uygulamanızın var olma nedeni olan tek işe kadar izlenen yol. Aşağıdaki satırlar StudyRoom'dan: **yalnızca giriş satırı herkes için aynıdır**; diğer satırlar kendi uygulamanızın ekranlarıdır.

| # | Ekran | Kullanıcı orada ne yapar | Gereksinimler |
|---|---|---|---|
| 1 | Giriş | e-posta adresini ve 4 haneli kodu girer | REQ-001, REQ-006 |
| 2 | Bugünün odaları | hangi odaların saat saat boş olduğunu görür | REQ-002, REQ-003 |

**Giriş dahil en az beş ekran.** Beş ekranı ve arkalarındaki gereksinimleri söyleyemiyorsanız proje henüz hazır değildir; bunu bugün fark etmek daha iyidir. 4. haftada her satır prototipinizin bir ekranı olur.

---

## Vaktiniz kalırsa

- Birbirinizin `must` gereksinimlerinin kabul ölçütlerini okuyun. Test edenin kontrol edemeyeceği her ölçütü işaretleyin; örneğin "kullanıcılar memnun kalır".
- Grubunuzun toplandığı haftalar için birbirinize nasıl ulaşacağınızı (bir mesajlaşma grubu) kararlaştırın.
- Ben buradayken Bölüm B'ye başlayın: §8'den ve §12'deki mağaza seçiminden.
- Mağaza seçiminiz kesin mi? Geliştirici hesabınızı (S1) şimdiden açabilirsiniz. Kimlik kontrolü günler sürer; S1 4. haftada notlanır.

---

## Bu grup kalıyor

Bugünkü grubunuz grubunuz olarak kalır. Her hafta **toplanmaz**: hangi haftalarda ve ne
için toplandığını her ödev söyler.

**4. hafta:** seçtiğiniz bir sınıf arkadaşınız, **collaborator**'ınız, test case'lerinizi prototipiniz üzerinde yürütür.

`weekNN/group_NN.json`, o haftanın ödevinin adını verdiği kişileri o haftanın rolüyle tutar: 4 collaborator · 5 kimse (tek başınıza çalışırsınız) · 6 attacker · 7 tester · 8 test-user · 9 beta-tester · 10 uat-participant · 11 release-tester · 12 poster-reviewer.

---

## Gereksinimler — id'ler kalıcı, liste açık

`requirements.json` hala değişebilir: ekleyin, yeniden yazın, çıkarın (id kalır, `"dropped": true`).

**Cumartesiden itibaren bir id'nin anlamı hiç değişmez.** `REQ-004` aralıkta da aynı şeyi ifade etmeli.

**Liste 5. haftanın sonuna kadar açık kalır.** 4. haftada kabul ölçütlerinizden test case'ler yazıp tıklanabilir prototip üzerinde yürütürsünüz; eksik çıkan her şey bir Change log satırıyla listeye girer.

**5. haftanın sonu: gereksinimler + test case'ler = taban çizginiz (baseline).** Sonra her değişiklik bir change request'tir: `CR-` ile başlayan bir Change log satırı.

REQ-001 (4 haneli e-posta koduyla giriş) ve REQ-006 (390 px telefon ekranı) herkes için aynıdır; ifadeyi ürününüze göre uyarlayın.

---

## Push

```bash
python .github/check_deliverables.py
git add .
git commit -m "week03: pitch, review, proposal revised, main flow"
git push
```

11:45'e dek push edin. Ders notu, dersin sonuna dek push ettiğiniz son commit'i okur. Push edilmemiş iş yok sayılır.

Derste: **10:00, 11:00 ve 11:45** civarında (±15 dakika) push edin; her push'ta yeni iş olsun.
Ders dışında: aralarında en az bir saat olan en az iki commit. **Asla force push yapmayın.**

---

## Cumartesi 23:59'a kadar — Bölüm B, §8–§12

Projenin neden yapmaya değer olduğunu söyleyen yarı. `PROPOSAL.md` içinde her bölüm için NEDEN / NE açıklaması ile zayıf ve güçlü birer örnek var.

- **§8 Pazar** — kim, kaç kişi, nereden biliyorsunuz. Beş test kullanıcınız ilk satırdır.
- **§9 Rakipler** — bugün bunu çözen üç şey. Bir kağıt liste de sayılır.
- **§10 Karşılaştırma** — *kullanıcının* ölçütleriyle küçük bir tablo ve tek cümle.
- **§11 Ticari potansiyel** — kendini nasıl finanse eder; gerekçesi varsa "ticari niyet yok, değeri X" demek de dürüst bir cevaptır.
- **§12 Riskler** — 11. haftaya kadar sizi durdurabilecek üç şey; her biri için bir plan ve bir yedek. **Mağazayı adlandırın** (S0): ücret, inceleme süresi. Önce `AI_PLATFORMS_AND_STORES_TR.md` dosyasını okuyun.

---

## Cumartesiye kadar — düşman gözüyle okutma, `week03/ai_log_03.md`

Bu hafta asistan, **hayır** demek isteyen yatırımcıyı oynar.

1. Bölüm B'nizi verin. Teklifinize özgü en güçlü üç itirazı isteyin.
2. Biri **haklı**: teklifte cevaplayın, Değişiklik günlüğüne yazın.
3. Biri **haksız**: nedenini gösterin — bir sayı, bir kaynak, kontrol ettiğiniz bir şey.
4. Yazışmayı yapıştırın.

"Yararlı geri bildirim verdi" puan getirmez. İyi itirazı kötüsünden ayırmak bir beceridir.

**Günlüğü kendiniz yazın.** Kanıt bloğu dışında asistan yok, dil için bile. Diliniz notlanmaz; asistanın yazdığı bir günlük en çok 1 puan alır.

---

## 3. hafta nasıl notlanıyor — 10 puan

| | Puan | Ne |
|---|---|---|
| Ders sonu (11:45) | 5 | sunum tam, üç değerlendiren gerçek cümlelerle, değişiklik günlüğü başlamış, beş ekran yazılmış |
| Cumartesi denetleyici | 2 | §8–§12 dolu, mağaza adlandırılmış, üç itirazlı ai_log |
| İnsan katkısı | 2 | ai_log ve kanıtı; arkasında gerçek kararlar olan incelemeler |
| Commit disiplini | 1 | 10:00, 11:00, 11:45 civarında push; ders dışında bir saat arayla iki commit |

Katkı bonusu: adını yazdığınız her değerlendiren haftalık notunuzun %10'unu kazanır; siz de verdiğiniz incelemeler için aynısını.

---

## Gelecek hafta: prototip ve test case'ler

**4. hafta:** ana akışınızın tıklanabilir bir prototipi ve kabul ölçütlerinizden yazılmış test case'ler.

Seçtiğiniz bir sınıf arkadaşınız, collaborator'ınız, test case'leri prototip üzerinde yürütür; çalışmayan her şey gereksinimlerde neyin eksik olduğunu gösterir.

**Gelecek haftaya kadar:** kabul ölçütlerinizi yeniden okuyun. Bir testçinin ne görmesi gerektiğini söylemeyen her ölçütü yeniden yazın.

---

## Sınıfla ilgili iki kural

**Bir öğrenci, bir bilgisayar, bir GitHub hesabı.** Arkadaşınızın bilgisayarında ya da onun
oturumunda yapılan iş ders için puan getirmez. Bilgisayarınızı şarjı dolu getirin.

**Yoklama sisteminde kayıtlı değilseniz gelmemiş sayılırsınız.** Ne push edilmiş olursa olsun, ders slotunun beş puanı o zaman gider.

---

## Şimdi

Gruplar kuruldu. Bilgisayarlar açık, `PITCH_03.md` önizlemede.

**Her grupta ilk sunan: başlayın.**

**Dersin sonunda (11:45) projenizin başlığı ve içeriği kesinleşiyor.** Gereken zamanı ayırın.

<!-- Saati başlat. Dolaş. Turdan sonra "Turdan sonra" slaydı 11:35'e kadar projeksiyonda kalsın; 11:35'ten sonra "Push". Not, dersin sonuna dek push edilen son commit'i okur: push.md blok 3. -->
