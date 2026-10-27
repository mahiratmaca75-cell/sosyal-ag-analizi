---

### 2. `sosyal-ag-analizi` Deposu İçin `README.md`

`sosyal-ag-analizi` deposuna girip aynı şekilde `README.md` oluştur ve yapıştır:

```markdown
# 🕸️ Sosyal Ağ Analizi: Bağımlılık & Etkileşim Grafı Modeli

Bu çalışma, paket bağımlılıkları ve geliştirici ekosistemleri arasındaki yapısal etkileşimleri ağ bilimi (Network Science) metrikleri kullanarak inceleyen bir sosyal ağ analizi projesidir.

---

## 🎯 Projenin Amacı ve Kapsamı
Yazılım ekosistemlerindeki kütüphanelerin birbirleriyle kurduğu yönlü/yönsüz bağlantı ağını graf teorisiyle modelleyerek; ağdaki merkezi aktörleri, kritik köprü düğümleri (bottlenecks) ve kümelenme yapılarını nicel verilerle ortaya koymak.

---

## 📊 Analiz Metrikleri ve Yöntem
Ağ yapısı Python (`networkx`, `matplotlib`) kütüphaneleri kullanılarak aşağıdaki metrikler ekseninde analiz edilmiştir:

- **Derece Merkeziliği (Degree Centrality):** Doğrudan en fazla bağımlılık ilişkisine sahip merkez paketler.
- **Arasındalık Merkeziliği (Betweenness Centrality):** Ağdaki bilgi/akış yolları üzerinde köprü görevi gören kritik düğümler.
- **Kümelenme Katsayısı (Clustering Coefficient):** Düğümlerin kendi aralarında ne derece alt topluluklar (modüler klikler) oluşturduğu.

---

## 📁 Depo İçeriği
- `npm_analiz.py`: Graf verilerini işleyen, ağ metriklerini hesaplayan ve görselleştirmeyi üreten ana analiz betiği.
- `npm_ag_grafigi.png`: Çıkarılan ağ topoğrafyasının görselleştirilmiş graf matrisi.
- `npm_analiz_sonuc_raporu.txt`: Düğüm dereceleri, yoğunluk matrisleri ve özet ağ bulgularını içeren metin raporu.

---

## ⚙️ Çalıştırma Adımları

```bash
# Depoyu klonlayın
git clone [https://github.com/mahiratmaca75-cell/sosyal-ag-analizi.git](https://github.com/mahiratmaca75-cell/sosyal-ag-analizi.git)

# Gerekli Python kütüphanelerini kurun
pip install networkx matplotlib pandas

# Analizi yürütün
python npm_analiz.py
