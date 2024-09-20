# İlaç Yan Etkileri Analizi
# Emir Erdem - eemireerdem@gmail.com

# Açıklama

Proje, hastalar tarafından kullanılan ilaçların yan etkilerini etkilerini analiz etmektedir. pandas, numpy, scikit-learn, missingno, matplotlib ve seaborn gibi Python kütüphanelerini kullanarak keşifsel veri analizi, özellik mühendisliği, veri ön işleme ve görselleştirmeleri kapsar.

# Kurulum ve Çalıştırma

**Projeyi yerel bir ortamda çalıştırmak için:**
 
 Projeyi klonla: git clone https://github.com/emirerdem/Pusula_Emir_Erdem.git
 
 Gerekli Python sürümünü ve gerekli kütüphanelerini yükleyin: pip install -r requirements.txt

 Boru hattını çalıştırmak için: pipeline("side_effect_data 1.xlsx")


# Genel Bakış



# Keşifsel Veri Analizi

- Veri setindeki eşsiz veriler, veri seti boyutu, verilerin tipleri gibi özelliklere baktım.

# Görselleştirme

- Verileri kategorik ve numerik olarak ayırdım. Önce görselleri veri işleme yapmadan görselleştirdim. Daha sonra veri işleyip yeni veriler ekledikten sonra tekrar görselleştirdim.

# Özellik Mühendisliği

- Elimizde olan verileri kullanarak yeni veriler ortaya çıkardım. Yaş özelliği, yaş özelliğini ve cinsiyet özelliğini kullanarak yeni bir cinsiyet yaş özelliği, yan etki çıkma süresi, ilaç kullanma süresi, vücut kitle indeksi gibi değişkenler ürettim.

# Eksik Verileri Doldurma

- Cinsiyet özelliğini en çok kullanılan veriye göre doldurdum. Yaş, boy ve kilo özelliklerini cinsiyet kırılımınıda göz önünde bulundurarak yaşların ortlaması ile doldurdum.

# Kategorik değişkenleri Sayısal Değişkene çevirdim

- İkili olan veri (cinsiyet) değişkenini LabelEncoder() ile çevirdim.
  Kardinalitesi yüksek olan verileri ise one_hot_encoder() fonksiyonu ile çevirdim.

# Sayısal değişkenleri Ölçekledim.

- Standart scaler tekniği ile verileri tekrardan ölçeklendirdim.
