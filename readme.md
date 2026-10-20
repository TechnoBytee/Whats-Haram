# İslam'da Haram Yiyecek ve İçecekler Veri Seti / Haram Foods & Drinks in Islam Dataset (JSON)

Bu depo (repository), İslam hukukuna (fıkıh) göre yenmesi ve içilmesi haram veya tahrimen mekruh olan yiyecekleri, içecekleri, hayvansal kısımları ve modern gıda katkı maddelerini **Türkçe (`tr`)** ve **İngilizce (`en`)** olarak yapılandırılmış biçimde sunan açık kaynaklı bir JSON veri setidir (`islamda_haram_yiyecek_ve_icecekler.json`).

This repository provides a comprehensive, structured, bilingual (**Turkish `tr`** and **English `en`**) JSON dataset (`islamda_haram_yiyecek_ve_icecekler.json`) of forbidden (haram) and strictly disliked (makruh tahrimi) foods, beverages, animal organs, and modern food additives in Islamic jurisprudence (Fiqh).

## Proje Hakkında / About the Project

* **Çift Dilli Yapı (Bilingual Support):** Tüm kategori başlıkları, madde adları, fıkhi hükümler, açıklamalar, örnek listeleri ve kaynak başlıkları hem Türkçe hem İngilizce olarak yapılandırılmıştır.
* **Klasik ve Çağdaş Fıkıh Sentezi (Classical & Contemporary Fiqh Synthesis):** Kur'an-ı Kerim ayetleri, sahih hadis kaynakları (Kütüb-i Sitte) ve temel fıkıh mezheplerinin (Hanefi, Şafii, Maliki, Hanbeli ve ilgili yerlerde Caferi) görüşleri bir arada sunulmuştur.
* **Mezhep Farklılıklarının Gösterimi (Madhhab Comparisons):** Deniz ürünleri (midye, karides, ıstakoz, yengeç), at eti veya suda kendiliğinden ölen balıklar gibi mezhepler arasında görüş ayrılığı bulunan konularda her mezhebin yaklaşımı açıkça belirtilmiştir.
* **Modern Gıda Sanayii ve E-Kodları (Food Additives & E-Numbers):** Jelatin (`E441`), Karmin (`E120`), emülgatörler (`E471`, `E322`, `E422`), L-Sistein (`E920`), peynir mayası (`rennet`) ve enzimler (`pepsin`, `lipaz`) gibi endüstriyel bileşenlerin kaynaklarına göre hükümleri detaylandırılmıştır.
* **Doğrulanabilir Resmi Kaynaklar (Verified Authoritative Sources):** Her bir madde; [T.C. Diyanet İşleri Başkanlığı Din İşleri Yüksek Kurulu](https://kurul.diyanet.gov.tr/), [Diyanet Kur'an Yolu Tefsiri](https://kuran.diyanet.gov.tr/), [American Halal Foundation](https://halalfoundation.org/) ve klasik fıkıh ansiklopedilerine ait doğrudan bağlantılarla (`source_urls`) desteklenmiştir.

## Veri Seti Kapsamı ve Kategoriler / Dataset Scope & Categories

Veri seti **7 ana kategori** ve **22 kapsamlı alt başlık** altında yüzlerce tekil gıda, içecek ve katkı maddesi örneğini barındırır:

| Kategori Kodu (`category_id`) | Kategori Adı (TR) | Category Name (EN) | Alt Başlık Sayısı | Kapsam Özeti |
| :--- | :--- | :--- | :---: | :--- |
| `CAT_01_QURANIC_EXPLICIT_PROHIBITIONS` | 1. Kur'an-ı Kerim'de Doğrudan (Nass İle) Haram Kılınan Hayvansal Gıdalar ve Kesim İhlalleri | 1. Animal Products and Slaughter Violations Explicitly Prohibited in the Quran | 5 | Domuz ve türevleri, akıtılmış kan, meyte (leş), boğulan/vurulan/düşen/boynuzlanan hayvanlar, Allah'tan başkası adına veya kasten besmelesiz kesilenler, fal okları ve ihram avı |
| `CAT_02_PROHIBITED_LAND_ANIMALS_AND_BIRDS` | 2. Sünnet ve Fıkıh İle Haram Kılınan Kara Hayvanları, Kuşlar ve Haşerat | 2. Land Animals, Birds, and Insects Prohibited by the Sunnah and Islamic Jurisprudence | 5 | Azı dişli yırtıcı kara hayvanları, pençeli yırtıcı ve leşçil kuşlar, evcil eşek ve katır (at eti ihtilafıyla), haşerat/böcekler/sürüngenler (çekirge istisnasıyla) ve pislik yiyen hayvanlar (`cellâle`) |
| `CAT_03_MARINE_AND_AQUATIC_ANIMALS` | 3. Deniz ve Su Hayvanlarında Haram Olanlar (İttifak Edilenler ve Mezhep İhtilafları) | 3. Prohibited Marine and Aquatic Animals (Consensus Rulings and Madhhab Differences) | 3 | Timsah, kurbağa, su yılanı ve kaplumbağa; balık dışındaki kabuklu ve yumuşakçalar (yengeç, ıstakoz, karides, midye, kalamar, ahtapot) ve suda kendiliğinden ölüp ters vuran balıklar (`tâfî`) |
| `CAT_04_INEDIBLE_ORGANS_OF_HALAL_ANIMALS` | 4. Eti Helal Olan Hayvanların Yenmesi Haram veya Tahrimen Mekruh Olan Organları | 4. Prohibited or Strictly Disliked (Makruh Tahrimi) Organs of Halal-Slaughtered Animals | 1 | İslami usulle kesilmiş helal hayvanların yenmeyen 7 kısmı: akıtılmış kan, erkeklik ve dişilik cinsel organları, husyeler (yumurtalar), idrar torbası, öd kesesi ve bezeler (guddeler) |
| `CAT_05_INTOXICANTS_DRINKS_AND_HARMFUL_SUBSTANCES` | 5. İçilmesi ve Tüketilmesi Haram Olan İçecekler, Alkollü Maddeler, Uyuşturucular ve Zehirler | 5. Prohibited Beverages, Alcoholic Intoxicants, Narcotics, and Harmful Substances | 6 | Alkollü içkiler (`hamr`), pişirme esnasında alkol katılan yemekler, içki olarak tüketilen sentetik alkol/kolonya, uyuşturucular, zehirler, sigara/tütün ürünleri, necis sıvılar, eti haram hayvanların sütleri ve insan eti/kanı |
| `CAT_06_HARAM_FOOD_ADDITIVES_AND_INGREDIENTS` | 6. Haram Kaynaklı Gıda Katkı Maddeleri ve İşlenmiş Gıda Bileşenleri | 6. Prohibited Food Additives and Processed Food Ingredients Derived from Haram Sources | 3 | Domuz veya gayri-helal kesim kaynaklı jelatin (`E441`), koşnil böceği boyası karmin (`E120`), domuz pepsini/lipazı, gayri-helal peynir mayası (`rennet`), hayvansal emülgatörler (`E471`, `E322`, `E422`) ve L-Sistein (`E920`) |
| `CAT_07_HARAM_LI_GHAYRIHI_AND_CONSUMPTION_MANNER` | 7. Elde Ediliş Yolu veya Tüketim Şekli Sebebiyle Haram Olanlar (`Haram li-Gayrihî`) | 7. Foods and Drinks Prohibited Due to Unlawful Acquisition or Manner of Consumption (`Haram li-Ghayrihi`) | 2 | Hırsızlık, gasp, rüşvet, faiz ve kumarla elde edilen gıdalar, sahibinin rızası olmadan alınan yiyecekler, altın ve gümüş kaplardan yeme-içme ve sağlığa zarar verecek boyutta aşırı tüketim/israf |

## Dosya ve Şema Yapısı / JSON Schema & Structure

`islamda_haram_yiyecek_ve_icecekler.json` dosyası kök düzeyde `metadata` ve `categories` olmak üzere iki ana nesneden oluşur:

```json
{
  "metadata": {
    "title": { "tr": "...", "en": "..." },
    "description": { "tr": "...", "en": "..." },
    "fundamental_principles": { "tr": "...", "en": "..." },
    "classification_of_haram": {
      "haram_li_aynihi": {
        "name": { "tr": "Haram li-aynihî (Haram li-zâtihî)", "en": "Haram li-aynihi (Intrinsically Haram)" },
        "definition": { "tr": "...", "en": "..." }
      },
      "haram_li_ghayrihi": {
        "name": { "tr": "Haram li-gayrihî", "en": "Haram li-ghayrihi (Extrinsically / Derivatively Haram)" },
        "definition": { "tr": "...", "en": "..." }
      }
    },
    "necessity_exception_darurah": { "tr": "...", "en": "..." },
    "research_sources": [
      {
        "id": "SRC_DIYANET_KARA_HAYVANLARI",
        "institution": "T.C. Diyanet İşleri Başkanlığı - Din İşleri Yüksek Kurulu",
        "title_tr": "Kara hayvanlarından eti yenilip yenilmeyenler hangileridir?",
        "title_en": "Which land animals are permissible and impermissible to eat?",
        "url": "https://kurul.diyanet.gov.tr/tr/fetva/kara-hayvanlarindan-eti-yenilip-yenilmeyenler-hangileridir/0198bc0e-e91d-75d3-a056-45ee437a90ff"
      }
    ]
  },
  "categories": [
    {
      "category_id": "CAT_01_QURANIC_EXPLICIT_PROHIBITIONS",
      "category_name": { "tr": "...", "en": "..." },
      "category_summary": { "tr": "...", "en": "..." },
      "items": [
        {
          "id": "ITEM_01_01",
          "name": {
            "tr": "Domuz ve Tüm Domuz Türevleri (Evcil ve Yaban Domuzu)",
            "en": "Pork and All Swine By-Products (Domestic Pig and Wild Boar)"
          },
          "arabic_term": "لحم الخنزير (Lahm al-Khinzir)",
          "ruling": {
            "tr": "Kesin Haram (Haram li-aynihî - İcma ile)",
            "en": "Strictly Haram (Intrinsically Haram by unanimous consensus)"
          },
          "examples": {
            "tr": ["Domuz eti...", "Domuz iç yağı (lard)..."],
            "en": ["Pork meat...", "Pig fat and suet (lard)..."]
          },
          "explanation": { "tr": "...", "en": "..." },
          "scriptural_evidence": [
            "Kur'an-ı Kerim: Bakara 2/173, Mâide 5/3, En'âm 6/145, Nahl 16/115",
            "Hadis: Buhârî, Büyû', 112; Müslim, Müsâkât, 71"
          ],
          "source_urls": [
            "https://kurul.diyanet.gov.tr/tr/fetva/kara-hayvanlarindan-eti-yenilip-yenilmeyenler-hangileridir/0198bc0e-e91d-75d3-a056-45ee437a90ff"
          ]
        }
      ]
    }
  ]
}
```

### Alan Açıklamaları / Field Reference

| Alan Adı (`Field`) | Veri Tipi (`Type`) | Açıklama (TR) | Description (EN) |
| :--- | :--- | :--- | :--- |
| `metadata.fundamental_principles` | `Object {tr, en}` | İslam fıkhındaki temel helallik (`ibâha-i asliyye`) ve temizlik (`tayyibât` / `habâis`) ilkesi | Core Islamic legal principle of original permissibility (`al-ibahah al-asliyyah`) |
| `metadata.classification_of_haram` | `Object` | `haram_li_aynihi` (özü itibarıyla haram) ve `haram_li_ghayrihi` (elde ediliş şekliyle haram) tanımları | Definitions of intrinsic (`li-aynihi`) vs. extrinsic (`li-ghayrihi`) prohibitions |
| `metadata.necessity_exception_darurah` | `Object {tr, en}` | Zaruret (ıztırar) halinde geçerli olan istisnai kurallar | Rules governing life-saving necessity (`darurah`) |
| `metadata.research_sources` | `Array<Object>` | Araştırmada kullanılan tüm resmi kaynakların kimliği, kurumu, başlığı ve URL'si | List of all verified primary and secondary research sources with URLs |
| `categories[].category_id` | `String` | Kategorinin benzersiz sabit tanımlayıcısı | Unique identifier for the category |
| `categories[].items[].id` | `String` | Alt maddenin benzersiz kimliği (`ITEM_01_01` vb.) | Unique identifier for the item (`ITEM_01_01`, etc.) |
| `categories[].items[].arabic_term` | `String` | İlgili hükmün veya maddenin klasik fıkıh literatüründeki Arapça terimi ve Latin harfli okunuşu | Classical Arabic jurisprudential term and transliteration |
| `categories[].items[].ruling` | `Object {tr, en}` | Maddenin dini hükmü ve varsa mezhepler arası görüş farkları | Religious ruling and any differences across madhhabs |
| `categories[].items[].examples` | `Object {tr[], en[]}` | Kategoriye giren somut hayvan, içecek, organ veya katkı maddesi örnekleri | Concrete examples of animals, beverages, organs, or food additives |
| `categories[].items[].scriptural_evidence` | `Array<String>` | Hükmün dayandığı Kur'an-ı Kerim sure/ayet numaraları ve hadis kaynakları | Quranic verses and Hadith collection references supporting the ruling |
| `categories[].items[].source_urls` | `Array<String>` | Maddeye ait resmi fetva, tefsir veya sertifikasyon sayfasının doğrudan bağlantıları | Direct URLs to official fatwas, tafsirs, or halal certification guides |

## Nasıl Kullanılır? / Usage Examples

### 1. Python ile Kullanım / Using with Python

Veri setini yükleyerek Türkçe veya İngilizce anahtar kelime (ör. `jelatin`, `E120`, `karides`, `alkol`) araması yapabilirsiniz:

```python
import json

with open("islamda_haram_yiyecek_ve_icecekler.json", "r", encoding="utf-8") as f:
    dataset = json.load(f)


def search_haram_items(query: str, lang: str = "tr"):
    """Verilen anahtar kelimeyi isim, açıklama ve örneklerde arar."""
    q = query.lower()
    results = []
    for category in dataset["categories"]:
        for item in category["items"]:
            name_text = item["name"][lang].lower()
            expl_text = item["explanation"][lang].lower()
            examples_list = [ex.lower() for ex in item["examples"][lang]]

            if (
                q in name_text
                or q in expl_text
                or any(q in ex for ex in examples_list)
            ):
                results.append({
                    "id": item["id"],
                    "category": category["category_name"][lang],
                    "name": item["name"][lang],
                    "ruling": item["ruling"][lang],
                    "sources": item["source_urls"],
                })
    return results


# Örnek 1: Türkçe 'E120' veya 'karmin' araması
for match in search_haram_items("E120", lang="tr"):
    print(f"[{match['id']}] {match['name']}")
    print(f"Hüküm: {match['ruling']}")
    print(f"Kaynaklar: {', '.join(match['sources'])}\n")

# Example 2: English search for 'shrimp' (madhhab comparison)
for match in search_haram_items("shrimp", lang="en"):
    print(f"[{match['id']}] {match['name']}")
    print(f"Ruling: {match['ruling']}\n")
```

### 2. JavaScript / Node.js ile Kullanım / Using with JavaScript & TypeScript

Web veya mobil uygulamalarda (React, Next.js, Vue, React Native vb.) doğrudan içe aktararak çok dilli (`tr` / `en`) sorgulama yapabilirsiniz:

```javascript
const fs = require('fs');

const data = JSON.parse(
  fs.readFileSync('./islamda_haram_yiyecek_ve_icecekler.json', 'utf8')
);

/**
 * Belirli bir dilde tüm kategorileri ve alt maddeleri listeler
 * @param {'tr' | 'en'} lang
 */
function getCategoriesByLanguage(lang = 'tr') {
  return data.categories.map((cat) => ({
    id: cat.category_id,
    title: cat.category_name[lang],
    summary: cat.category_summary[lang],
    items: cat.items.map((item) => ({
      id: item.id,
      name: item.name[lang],
      arabicTerm: item.arabic_term,
      ruling: item.ruling[lang],
      examples: item.examples[lang],
      evidences: item.scriptural_evidence,
      sources: item.source_urls,
    })),
  }));
}

console.log(JSON.stringify(getCategoriesByLanguage('tr')[0], null, 2));
```

### 3. Komut Satırında (`jq`) Kullanım / Querying via CLI (`jq`)

Terminal üzerinden `jq` aracını kullanarak veri setini hızlıca filtreleyebilirsiniz:

```bash
# Tüm ana kategori başlıklarını Türkçe ve İngilizce olarak listele
jq '.categories[] | {id: .category_id, tr: .category_name.tr, en: .category_name.en}' islamda_haram_yiyecek_ve_icecekler.json

# Gıda katkı maddeleri kategorisindeki (CAT_06) tüm maddeleri ve hükümlerini getir
jq '.categories[] | select(.category_id == "CAT_06_HARAM_FOOD_ADDITIVES_AND_INGREDIENTS") | .items[] | {name_tr: .name.tr, ruling_tr: .ruling.tr}' islamda_haram_yiyecek_ve_icecekler.json

# Veri setinde kullanılan tüm resmi araştırma kaynaklarını listele
jq '.metadata.research_sources[] | {id, institution, url}' islamda_haram_yiyecek_ve_icecekler.json
```

## Fıkhi Metodoloji ve Temel İlkeler / Jurisprudential Methodology

Veri seti hazırlanırken İslam hukukunun (Usûl-i Fıkıh) şu temel kaideleri esas alınmıştır:

1. **Eşyada Aslolan İbâhadır (`el-İbâhatü'l-Asliyye`):** Kur'an ve Sünnet'te haramlığına dair açık bir delil bulunmayan, temiz ve sağlığa yararlı (`tayyibât`) her gıda helal; pis, iğrenç, sarhoş edici veya sağlığa zararlı (`habâis`) olanlar ise haramdır ([Bakara 2/168, 173](https://kuran.diyanet.gov.tr/tefsir/Bakara-suresi/180/173-ayet-tefsiri); [En'âm 6/145](https://kuran.diyanet.gov.tr/tefsir/En'%C3%A2m-suresi/934/145-ayet-tefsiri)).
2. **Haram li-aynihî ve Haram li-gayrihî Ayrımı:** Domuz eti, akıtılmış kan, leş (`meyte`) ve şarap (`hamr`) gibi maddeler bizzat kendi özleri sebebiyle haramdır (`haram li-aynihî`). Özü itibarıyla helal olan bir gıdanın çalıntı, gasp, rüşvet veya faiz yoluyla elde edilmesi ise dışsal bir sebepten ötürü haramdır (`haram li-gayrihî`) ([Diyanet Haber – Haramın Çeşitleri](https://www.diyanethaber.com.tr/haramin-cesitleri-nelerdir)).
3. **İstihâle (Kimyasal Dönüşüm) İlkesi:** Haram veya necis bir maddenin yapısal/kimyasal değişime uğrayarak tamamen başka bir temiz maddeye dönüşmesi durumunda hükmü de değişir. Örneğin şarabın kendiliğinden veya müdahaleyle tamamen sirkeye dönüşmesi helaldir; ancak yemek pişirirken içine katılan şarap istihâleye uğramadığı için yemeği haram kılar ([Din İşleri Yüksek Kurulu – Yemekte Alkol Fetvası](https://kurul.diyanet.gov.tr/tr/fetva/yiyecekler-pisirilirken-sarap-gibi-alkollu-iceceklerin/0193c42d-a9f2-7fad-8f08-bf81a23dd46e)).
4. **Zaruret Hali (`Iztırar` / `Darurah`):** Açlıktan veya susuzluktan ölme tehlikesi bulunan ya da hayati bir hastalığın tedavisi için helal alternatif bulamayan kimse, başkasının hakkına tecavüz etmemek ve ölmeyecek/tedavi olacak miktarı aşmamak kaydıyla haram maddelerden tüketebilir ([Mâide 5/3](https://kuran.diyanet.gov.tr/tefsir/M%C3%A2ide-suresi/672/3-ayet-tefsiri); [Din İşleri Yüksek Kurulu – Tedavide Haram Madde Kullanımı](https://kurul.diyanet.gov.tr/tr/fetva/kullanilmasi-veya-yenilmesi-haram-bir-maddenin-ya-da/0193c42d-9abb-735d-31d9-b49358351387)).

## Araştırma Kaynakları ve Referanslar / Research Sources & References

Veri setindeki tüm maddeler aşağıdaki **20 resmi ve akademik kaynaktan** doğrulanarak derlenmiştir:

| Kaynak Kodu (`id`) | Kurum / Yayıncı | Kaynak Başlığı ve Doğrudan Bağlantı |
| :--- | :--- | :--- |
| `SRC_KURAN_BAKARA_173` | T.C. Diyanet İşleri Başkanlığı – Kur'an Yolu Tefsiri | [Bakara Suresi 173. Ayet ve Tefsiri](https://kuran.diyanet.gov.tr/tefsir/Bakara-suresi/180/173-ayet-tefsiri) |
| `SRC_KURAN_MAIDE_3` | T.C. Diyanet İşleri Başkanlığı – Kur'an Yolu Tefsiri | [Mâide Suresi 3. Ayet ve Tefsiri](https://kuran.diyanet.gov.tr/tefsir/M%C3%A2ide-suresi/672/3-ayet-tefsiri) |
| `SRC_KURAN_ENAM_145` | T.C. Diyanet İşleri Başkanlığı – Kur'an Yolu Tefsiri | [En'âm Suresi 145. Ayet ve Tefsiri](https://kuran.diyanet.gov.tr/tefsir/En'%C3%A2m-suresi/934/145-ayet-tefsiri) |
| `SRC_KURAN_MAIDE_90_91` | T.C. Diyanet İşleri Başkanlığı – Kur'an Yolu Tefsiri | [Mâide Suresi 90-91. Ayetler ve Tefsiri (İçki ve Kumar Yasağı)](https://kuran.diyanet.gov.tr/tefsir/M%C3%A2ide-suresi/759/90-91-ayet-tefsiri) |
| `SRC_DIYANET_KARA_HAYVANLARI` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Kara hayvanlarından eti yenilip yenilmeyenler hangileridir?](https://kurul.diyanet.gov.tr/tr/fetva/kara-hayvanlarindan-eti-yenilip-yenilmeyenler-hangileridir/0198bc0e-e91d-75d3-a056-45ee437a90ff) |
| `SRC_DIYANET_DENIZ_URUNLERI` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Yengeç, ıstakoz, karides, kalamar ve midye gibi deniz ürünleri yenir mi?](https://kurul.diyanet.gov.tr/tr/fetva/yengec-istakoz-karides-kalamar-ve-midye-gibi-deniz-urunleri/0198bc12-9106-7f6d-b2d3-2beaa72b6fce) |
| `SRC_DIYANET_YENMEYEN_ORGANLAR` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Bir hayvanın yenilmeyecek yerleri nerelerdir? Bu organların ne yapılması gerekir?](https://kurul.diyanet.gov.tr/tr/fetva/bir-hayvanin-yenilmeyecek-yerleri-nerelerdir-bu-organlarin/0193c42d-7e8d-731a-2e74-9974f7d95856) |
| `SRC_DIYANET_KESIM_SARTLARI` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Hayvan kesecek kimselerde bulunması gereken şartlar nelerdir?](https://kurul.diyanet.gov.tr/tr/fetva/hayvan-kesecek-kimselerde-bulunmasi-gereken-sartlar-nelerdir/0193c42d-9a4c-7695-365c-51ebf9a2f72e) |
| `SRC_DIYANET_AT_ETI` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [At eti helal midir?](https://kurul.diyanet.gov.tr/tr/fetva/at-eti-helal-midir/0193c42d-99ef-7a0a-deee-39e86f92e7fb) |
| `SRC_DIYANET_ESEK_SUTU` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Eşek sütünün tedavi maksatlı içilmesi caiz midir?](https://kurul.diyanet.gov.tr/tr/fetva/esek-sutunun-tedavi-maksatli-icilmesi-caiz-midir/0193c42d-aac4-7015-24b6-9bdf63f7fd17) |
| `SRC_DIYANET_YEMEKTE_ALKOL` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Yiyecekler pişirilirken şarap gibi alkollü içeceklerin katılması caiz midir?](https://kurul.diyanet.gov.tr/tr/fetva/yiyecekler-pisirilirken-sarap-gibi-alkollu-iceceklerin/0193c42d-a9f2-7fad-8f08-bf81a23dd46e) |
| `SRC_DIYANET_SENTETIK_ALKOL` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Üretim Aşamalarında Sentetik Alkol Kullanımının Hükmü Nedir?](https://kurul.diyanet.gov.tr/tr/fetva/uretim-asamalarinda-sentetik-alkol-kullaniminin-hukmu-nedir/0193c42d-b6f3-750b-466b-3e8585270328) |
| `SRC_DIYANET_SIGARA` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Sigara içmenin dini hükmü nedir?](https://kurul.diyanet.gov.tr/tr/fetva/sigara-icmenin-dini-hukmu-nedir/0193c42d-b845-70df-5e8c-44ed6a000be4) |
| `SRC_DIYANET_TEDAVIDE_HARAM` | T.C. Diyanet İşleri Başkanlığı – Din İşleri Yüksek Kurulu | [Kullanılması veya yenilmesi haram bir maddenin ya da bunlardan imal edilen ilaçların tedavide kullanılması caiz midir?](https://kurul.diyanet.gov.tr/tr/fetva/kullanilmasi-veya-yenilmesi-haram-bir-maddenin-ya-da/0193c42d-9abb-735d-31d9-b49358351387) |
| `SRC_DIYANET_HABER_HARAM_CESITLERI` | Diyanet Haber / DİB İslam İlmihali | [Haramın çeşitleri nelerdir? (Haram li-aynihî ve Haram li-gayrihî)](https://www.diyanethaber.com.tr/haramin-cesitleri-nelerdir) |
| `SRC_AHF_FORBIDDEN_FOODS` | American Halal Foundation (AHF) | [What Can Muslims Not Eat? Guide to Islamic Dietary Laws](https://halalfoundation.org/what-can-muslim-not-eat/) |
| `SRC_AHF_INGREDIENTS` | American Halal Foundation (AHF) | [A Comprehensive Guide to Halal and Haram Ingredients](https://halalfoundation.org/halal-and-haram-ingredients-list/) |
| `SRC_ISLAMQA_INSECTS` | IslamQA (İmam Nevevî, *el-Mecmû'* referanslı) | [Are Insects Halal? Ruling on Eating Insects, Vermin and Rodents](https://islamqa.info/en/answers/21901/are-insects-halal) |
| `SRC_JELATIN_DIYANET_SUMMARY` | Oye Teknoloji (Din İşleri Yüksek Kurulu 18.08.2017 Jelatin Kararı Özeti) | [Jelatin helal mi? Diyanet Din İşleri Yüksek Kurulu Değerlendirmesi](https://oyeteknoloji.com/tr/blog/is-gelatin-halal/) |
| `SRC_WIKIPEDIA_ISLAMIC_DIETARY_LAWS` | Wikipedia / Akademik Fıkıh Özeti ve İstanbul Üniversitesi İlahiyat Fakültesi Tezi | [Islamic Dietary Laws](https://en.wikipedia.org/wiki/Islamic_dietary_laws) & [Kur'an'a Göre Hayvansal Gıdalarda Helallik Ölçüleri Tezi](https://nek.istanbul.edu.tr/ekos/TEZ/51118.pdf) |

## Katkıda Bulunma / Contributing

Veri setine yeni katkı maddeleri (E-kodları), farklı mezhep görüşleri veya ek dil destekleri eklemek isterseniz şu adımları izleyebilirsiniz:

1. Bu depoyu forklayın (`Fork`).
2. Yeni bir özellik dalı oluşturun (`git checkout -b feature/yeni-katki-maddesi`).
3. Eklediğiniz her hüküm için mutlaka resmi bir fetva kurulu, tefsir veya akademik fıkıh kaynağını `scriptural_evidence` ve `source_urls` alanlarına ekleyin.
4. JSON formatının geçerliliğini doğrulayın (`python3 -m json.tool islamda_haram_yiyecek_ve_icecekler.json > /dev/null`).
5. Değişikliklerinizi commit edin ve bir **Pull Request (PR)** açın.

## Yasal Uyarı ve Lisans / Disclaimer & License

* **Bilgilendirme Notu (Disclaimer):** Bu veri seti eğitim, akademik araştırma ve yazılım geliştirme (barkod/içerik analiz uygulamaları, helal gıda doğrulama araçları vb.) amacıyla derlenmiştir. Özel tıbbi zaruret halleri ve karmaşık endüstriyel girdi soruları için [T.C. Diyanet İşleri Başkanlığı Din İşleri Yüksek Kurulu](https://kurul.diyanet.gov.tr/) veya yetkili helal sertifikasyon kurumlarına başvurulmalıdır.
* **Lisans (License):** Bu proje açık kaynaklı olup **MIT Lisansı (MIT License)** altında kullanıma sunulmuştur. Kaynak göstermek suretiyle ticari ve kişisel projelerde özgürce kullanılabilir.
