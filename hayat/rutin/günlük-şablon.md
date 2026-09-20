<%* 
let tarih = tp.file.title;
let gun = window.moment(tarih, "YYYY-MM-DD").format("dddd");
let dersler = "";
if (gun === "Salı") {
  dersler = "- [ ] Örnekleme 1 (09:00)\n- [ ] Mat. Analiz 3 (13:00)\n- [ ] Bilg. Prog. Online (16:00)\n- [ ] 💪 Bacak (17:00)";
} else if (gun === "Çarşamba") {
  dersler = "- [ ] Mat. İstatistik (09:00)\n- [ ] Sosyal Sor. (14:00)";
} else if (gun === "Perşembe") {
  dersler = "- [ ] Mat. Analiz 3 (11:00)\n- [ ] Mesleki İngilizce (13:00)";
} else if (gun === "Cuma") {
  dersler = "- [ ] 💪 İtiş (11:00)";
} else if (gun === "Pazartesi") {
  dersler = "- [ ] 💪 İtiş (11:00)";
} else {
  dersler = "- Hafta sonu";
}
%>
# <% tp.file.title %>

## 🌅 Sabah
- [ ] Duş
- [ ] Kahvaltı
- [ ] Günü planla (5 dk)

## 📚 Dersler
<%* tR += dersler; %>

## ✅ Görevler
- [ ] 
- [ ] 
- [ ] 

## 🌙 Akşam
- [ ] Yarını planla (5 dk)
- [ ] Yansıma: bugün nasıldı?