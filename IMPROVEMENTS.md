# GitHub Stats va Metrics Yaxshilanishlari / GitHub Stats and Metrics Improvements

## 📋 O'zgartirishlar Haqida / About Changes

### Uzbekcha / Uzbek

Ushbu PR GitHub profil README.md faylidagi statistika va metrikalarni yaxshilaydi va ishonchli qiladi.

#### Asosiy Muammolar va Yechimlar:

1. **GitHub Stats va Top Languages Ko'rinmaydi**
   - **Muammo**: Statik rasmlar ba'zida yuklanmaydi yoki eskirgan ma'lumotlarni ko'rsatadi
   - **Yechim**: 
     - `<picture>` teglari qo'shildi (dark mode uchun fallback)
     - `cache_seconds=1800` parametri qo'shildi (30 daqiqa kesh)
     - `include_all_commits=true` qo'shildi (barcha commitlarni ko'rsatish)
     - `hide=Jupyter%20Notebook` qo'shildi (kerakli bo'lmagan tillarni yashirish)

2. **Yangi Metrics Qo'shildi**
   - **GitHub Profile Summary Cards**: To'liq profil ma'lumotlari, til statistikasi, productive time
   - **Advanced Metrics**: lowlighter/metrics action bilan batafsil profil ma'lumotlari
   - **WakaTime Integration**: Coding vaqti statistikasi (agar API key sozlangan bo'lsa)

3. **Workflow Yaxshilanishlari**
   - **metrics.yml**: Har 6 soatda yangi comprehensive metrics yaratadi
   - **wakatime.yml**: WakaTime ma'lumotlarini avtomatik yangilaydi
   - **stats.yml**: Mavjud custom stats workflow'i saqlanib qolindi

#### Yangi Qo'shilgan Funksiyalar:

✅ **Reliable Stats Display**: Picture teglari bilan dark mode support
✅ **Detailed Metrics Section**: 5 xil summary card
✅ **Advanced Metrics**: 70+ qator comprehensive metrics workflow
✅ **WakaTime Integration**: Coding time tracking
✅ **Auto-update**: Har 6 soatda avtomatik yangilanish

---

### English

This PR improves and makes reliable the statistics and metrics in the GitHub profile README.md file.

#### Main Problems and Solutions:

1. **GitHub Stats and Top Languages Not Showing**
   - **Problem**: Static images sometimes don't load or show outdated data
   - **Solution**: 
     - Added `<picture>` tags (fallback for dark mode)
     - Added `cache_seconds=1800` parameter (30-minute cache)
     - Added `include_all_commits=true` (show all commits)
     - Added `hide=Jupyter%20Notebook` (hide unnecessary languages)

2. **New Metrics Added**
   - **GitHub Profile Summary Cards**: Full profile details, language stats, productive time
   - **Advanced Metrics**: Detailed profile information with lowlighter/metrics action
   - **WakaTime Integration**: Coding time statistics (if API key is configured)

3. **Workflow Improvements**
   - **metrics.yml**: Creates new comprehensive metrics every 6 hours
   - **wakatime.yml**: Automatically updates WakaTime data
   - **stats.yml**: Existing custom stats workflow preserved

#### New Features Added:

✅ **Reliable Stats Display**: Dark mode support with picture tags
✅ **Detailed Metrics Section**: 5 different summary cards
✅ **Advanced Metrics**: 70+ line comprehensive metrics workflow
✅ **WakaTime Integration**: Coding time tracking
✅ **Auto-update**: Automatic refresh every 6 hours

---

## 📝 Fayllardagi O'zgarishlar / File Changes

### 1. README.md
- GitHub Stats section yangilandi (picture tags, cache, parameters)
- Yangi "Detailed Metrics" section qo'shildi
- Yangi "Advanced Metrics" section qo'shildi
- WakaTime placeholder qo'shildi
- STATS:START/END commentlari qo'shildi (auto-update uchun)

### 2. .github/workflows/metrics.yml (YANGI)
- lowlighter/metrics action
- 15+ plugin yoqilgan
- Har 6 soatda yangilanadi
- Comprehensive profil statistikasi

### 3. .github/workflows/wakatime.yml
- actions/checkout@v3 qo'shildi
- SHOW_TITLE, SHOW_TIME, SHOW_TOTAL parametrlari qo'shildi

---

## 🚀 Ishlatish / Usage

### Avtomatik Yangilanish / Auto Update
Barcha workflow'lar avtomatik ishlaydi:
- **metrics.yml**: Har 6 soatda
- **wakatime.yml**: Har kuni yarim tunda
- **stats.yml**: Har kuni yarim tunda

### Qo'lda Ishga Tushirish / Manual Trigger
GitHub Actions → Workflows → "Run workflow" tugmasini bosing

### WakaTime Sozlash / WakaTime Setup
1. [WakaTime](https://wakatime.com) da akkaunt yarating
2. API key oling
3. Repository Settings → Secrets → New secret
4. Nom: `WAKATIME_API_KEY`
5. Value: sizning API key

---

## 🔧 Texnik Tafsilotlar / Technical Details

### Yangi URL Parametrlari / New URL Parameters:
- `cache_seconds=1800`: 30 daqiqalik kesh
- `include_all_commits=true`: Barcha commitlar
- `date_format=M%20j%5B%2C%20Y%5D`: Sana formati
- `hide=Jupyter%20Notebook`: Yashirilgan tillar
- `utcOffset=5`: Toshkent vaqti (UTC+5)

### Plugin'lar (metrics.yml):
- ✅ Languages analysis
- ✅ Follow-up (issues/PRs)
- ✅ Reactions
- ✅ Achievements
- ✅ Notable contributions
- ✅ Activity timeline
- ✅ Traffic
- ✅ Code snippet
- ✅ Lines of code

---

## 📊 Natijalar / Results

### Yaxshilangan Ko'rinish / Improved Display:
1. ✅ GitHub stats har doim ko'rinadi
2. ✅ Top languages har doim ko'rinadi
3. ✅ 5 qo'shimcha detailed metrics card
4. ✅ Advanced metrics SVG fayl
5. ✅ WakaTime coding stats (agar sozlangan bo'lsa)
6. ✅ Auto-refresh har 6 soatda

### Performance:
- Cache-enabled images (tezroq yuklanish)
- Optimized refresh intervals
- Fallback images (dark mode support)

---

## 🎯 Keyingi Qadamlar / Next Steps

1. **WakaTime API Key Sozlash** (agar kerak bo'lsa)
   - Repository secrets ga qo'shing
   - Workflow avtomatik ishlaydi

2. **Workflow'larni Monitoring Qilish**
   - GitHub Actions tab'da status tekshiring
   - Xatolar bo'lsa logs ko'ring

3. **Customize Metrics**
   - metrics.yml da plugin'larni o'zgartiring
   - README.md da display tartibini o'zgartiring

---

## 📞 Yordam / Support

Savollar yoki muammolar bo'lsa:
1. GitHub Issues orqali xabar bering
2. Pull Request ga comment qoldiring
3. Telegram: [@as1lbek_2706](https://t.me/as1lbek_2706)

---

**🎉 Tabriklaymiz! GitHub profilingiz endi professional va ishonchli metrikalar bilan jihozlangan!**

**🎉 Congratulations! Your GitHub profile is now equipped with professional and reliable metrics!**
