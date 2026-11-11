# Quran for Obsidian

A comprehensive, offline-first Quran plugin for Obsidian that enables you to instantly search, navigate, and insert Ayahs, Surahs, and full Quranic pages in both Block (Callout/Blockquote) and Inline formats.

Featuring embedded high-precision Uthmanic typography (**KFGQPC Hafs Uthmanic Script**), intelligent search normalization, contextual Ayah exploration, and dedicated note creation.

---

## 🌟 Key Features

### 1. Advanced Search Engine
* **Orthography & Script Normalization:** Seamlessly searches text ignoring Arabic/Persian letter variations (`ک/ك`, `ی/ي/ى`, Alef variants `ا/أ/إ/آ/ٱ`, Ta Marbuta `ة/ه`, Tashkeel/diacritics, and small Quranic diacritics).
* **Uthmanic Script Resolution:** Handles archaic/Quranic spelling variants where letters are omitted or written differently (e.g., searching for `ابراهیم` matches `إبراهيم` written as `إبرٲهم`, and `سماعون` matches `سمعون`).
* **Conjunction Handling:** Intelligent handling of the conjunction Waw (`و`) attached to Quranic words.
* **Exact & Fuzzy Relevance Scoring:** Prioritizes exact phrase matches, token matches, and word-boundary alignments.
* **Search Result Highlighting:** Dynamic match highlighting in the search suggestion dropdown.

### 2. Multi-Mode Insertion
* **Ayah Search (`Insert Ayah`):**
  * Search by text query (e.g., `الله نور السموات`).
  * Search by numerical reference: `Surah:Ayah` (e.g., `2:255` or `15:49`).
  * Search by Ayah Range: `Surah:Start-End` (e.g., `15:49-54` or `2:1-5`).
  * Search by Surah name & Ayah: Supports Arabic, Persian, and English transliterations (e.g., `حجر 49`, `حجر 49-54`, `Yaseen 12`, `Mulk 15-25`).
* **Surah Insertion (`Insert Surah`):**
  * Search by Surah name, transliteration, or revelation order/chronology.
  * Inserts the full Surah with proper basmala handling and Ayah separators.
* **Page Insertion (`Insert Page`):**
  * Search Quran pages by standard Madinah Mushaf numbering (`1` to `604`).
  * Quick sub-modal allows inserting the **entire page** at once or selecting a specific Ayah from that page.

### 3. Interactive Context Explorer (Surrounding Ayahs Modal)
* Selecting an Ayah from a text search opens a **20-Ayah contextual window** (10 Ayahs before and 10 Ayahs after).
* Navigate through surrounding verses using `↑` / `↓`.
* Select a multi-verse range directly in the context view using `Shift + ↑` / `Shift + ↓`.
* Press `Enter` to insert the selected range or single verse.

### 4. Inline vs. Block Output
* **Enter (`↵`):** Inserts the verse as a block (Callout or Blockquote based on plugin settings).
* **Mod + Enter (`Ctrl + Enter` / `Cmd + Enter`):** Inserts the verse **inline** directly inside your running sentences/paragraphs with customary end-of-verse decorative brackets.

### 5. Dedicated Ayah Note Creation
* Quickly generate independent Ayah notes inside a specified vault directory.
* Configurable naming patterns: `surah-ayah`, `surah/ayah`, `arabic-ayah`, `arabic/ayah`.
* Automatically includes customizable frontmatter tags and bidirectional links to the parent Surah note.

### 6. Authentic Uthmanic Typography
* Comes packaged with the authentic **KFGQPC Uthmanic Hafs Font** embedded directly in CSS (`qpc-hafs`), rendering end-of-ayah symbols and Waqf marks with perfect fidelity.

---

## ⌨️ Shortcuts & Hotkeys

| Action | Context | Shortcut |
| :--- | :--- | :--- |
| **Insert Block** | Any Search Modal | `Enter` (`↵`) |
| **Insert Inline** | Any Search Modal | `Ctrl + Enter` / `Cmd + Enter` |
| **Navigate Verses** | Surrounding Ayahs Modal | `↑` / `↓` |
| **Expand Range Selection** | Surrounding Ayahs Modal | `Shift + ↑` / `Shift + ↓` |
| **Close / Cancel** | Any Modal | `Esc` |

---

## ⚙️ Configuration & Settings

Access settings via **Settings > Quran**:

* **Output Format:**
  * `Callout`: Wraps verses in Obsidian Markdown callouts (`> [!quran-ayah] ...`).
  * `Blockquote`: Wraps verses in standard Markdown blockquotes (`> ...`).
  * `Inline`: Default output mode for inline insertion.
* **Callout Type:** Choose custom callout types (e.g., `quran`, `quran-ayah`, `quran-surah`, `note`, `quote`, etc.).
* **Ayah Note Folder:** Specify the folder path for newly generated Ayah notes (supports folder autosuggest).
* **Ayah Note Path Pattern:** Format filenames using English or Arabic Surah names, with hyphenated or folder structures.
* **Ayah Note Tags:** Comma-separated tags added automatically to the note frontmatter.
* **Link to Surah:** Automatically prepend a bidirectional wikilink (`[[Surah Name]]`) to the Ayah note metadata.

---
---

# افزونه قرآن برای آبسیدین (فارسی)

افزونه جامع و آفلاین قرآن کریم برای محیط ابسیدین (Obsidian)، طراحی‌شده برای پژوهشگران، یادداشت‌برداران و علاقه‌مندانی که نیازمند جستجوی سریع، مطالعه بافتی و درج آیات، سوره‌ها و صفحات قرآن در یادداشت‌های خود هستند.

این افزونه از رسم‌الخط عثمان‌طه و قلم رسمی مجمع ملک فهد (`qpc-hafs`) به صورت توکار بهره برده و نتایج را با نهایت دقت متنی و ظاهری ارائه می‌دهد.

---

## ✨ قابلیت‌های کلیدی

### ۱. جستجوی پیشرفته و هوشمند متنی
* **یکسان‌سازی حروف فارسی و عربی:** عدم حساسیت جستجو به تفاوت‌های نوشتاری مانند `ک` و `ك`، `ی`، `ي` و `ى`، انواع همزه و الف (`ا/أ/إ/آ/ٱ`) و تاء گرد (`ة/ه`).
* **انطباق با رسم‌الخط عثمانی:** شناسایی هوشمند کلماتی که در رسم‌الخط دارای الف مقصوره یا حذفیات خطی هستند (مانند جستجوی `ابراهیم` برای `إبرٲهم` یا `سماعون` برای `سمعون` و واژگانی نظیر `صلوة` و `زکوة`).
* **پشتیبانی از واو عطف متصل و منفصل:** مدیریت هوشمند واژگانی که با یا بدون واو تایپ می‌شوند.
* **هایلایت هوشمند عبارات یافته‌شده:** نمایش کلمات منطبق در متن آیه با برجسته‌سازی متنی داخل منوی جستجو.

### ۲. شیوه‌های متنوع فراخوانی و درج
* **درج آیه (`Insert Ayah`):**
  * جستجو با وارد کردن بخشی از متن آیه.
  * جستجو با آدرس عددی سوره و آیه (مانند `2:255` یا `15:49`).
  * جستجوی بازه‌ای از آیات با آدرس عددی (مانند `15:49-54`).
  * جستجو با نام سوره (فارسی/عربی/انگلیسی) و شماره آیه یا بازه (مانند `حجر 49` یا `حجر 49-54` یا `Mulk 1-5`).
* **درج سوره کامل (`Insert Surah`):**
  * جستجوی نام سوره و درج یکپارچه آن به همراه بسم‌الله و شماره‌گذاری آیات.
* **درج صفحه مصحف (`Insert Page`):**
  * جستجوی شماره صفحه (از ۱ تا ۶۰۴ عثمان‌طه).
  * امکان درج **کل صفحه به صورت یکجا** یا انتخاب یک آیه بخصوص از آن صفحه.

### ۳. پنجره ناوبری بافت آیات (Surrounding Context View)
* در صورت جستجوی متنی، پس از انتخاب آیه با کلید `Enter`، پنجره‌ای اختصاصی شامل **۲۰ آیه پیرامونی** (۱۰ آیه قبل و ۱۰ آیه بعد) باز می‌شود.
* پیمایش بین آیات با کلیدهای جهت‌نما (`↑` / `↓`).
* امکان **انتخاب چند آیه متوالی** با نگه داشتن `Shift` و زدن کلیدهای جهت‌نما (`Shift + ↑ / ↓`).
* زدن کلید `Enter` بازه انتخاب‌شده را بلافاصله در یادداشت درج می‌کند.

### ۴. درج بلوکی در برابر درج درون‌متنی (Inline)
* **کلید `Enter`:** درج آیه یا آیات به صورت بلوک ساخت‌یافته (Callout یا Blockquote مطابق تنظیمات).
* **کلید ترکیبی `Ctrl + Enter` (یا `Cmd + Enter`):** درج مستقیم آیه در همان خط و میان متن یادداشت جاری به همراه نماد شماره آیه.

### ۵. ساخت خودکار یادداشت اختصاصی برای آیه (Ayah Note)
* ساخت یک فایل مجزا برای آیه انتخاب‌شده از طریق دستور یا آیکون روبان `Create Ayah Note`.
* تعیین ساختار پوشه‌بندی و نام‌گذاری فایل (پوشه مجزا برای هر سوره یا نام‌گذاری پیوسته با خط تیره).
* قابلیت درج خودکار تگ‌ها (Tags) و پیوند به یادداشت والد سوره در بخش Frontmatter.

### ۶. قلم اصیل عثمان‌طه
* بهره‌گیری از قلم بهینه‌سازی‌شده **مجمع ملک فهد (Hafs Uthmanic)** درون استایل‌های افزونه، تضمین‌کننده نمایش درست اعراب، علائم وقف و گل آیات بدون نیاز به نصب فونت روی سیستم‌عامل.

---

## ⌨️ کلیدهای میانبر و کنترل‌ها

| عملکرد | محیط کاربری | کلید میانبر |
| :--- | :--- | :--- |
| **درج بلوکی (کال‌اوت/نقل‌قول)** | تمامی پنجره‌های جستجو | `Enter` (`↵`) |
| **درج درون‌متنی (Inline)** | تمامی پنجره‌های جستجو | `Ctrl + Enter` / `Cmd + Enter` |
| **پیمایش آیه به آیه** | پنجره بافت آیات پیرامونی | `↑` / `↓` |
| **انتخاب بازه‌ای از آیات** | پنجره بافت آیات پیرامونی | `Shift + ↑` / `Shift + ↓` |
| **انصراف و خروج** | تمامی پنجره‌ها | `Esc` |

---

## ⚙️ تنظیمات افزونه (Settings)

از مسیر **Settings > Quran** می‌توانید گزینه‌های زیر را پیکربندی کنید:

1. **Output Format:** انتخاب فرمت پیش‌فرض درج میان `Callout`، `Blockquote` یا `Inline`.
2. **Callout Type:** تعیین نوع کال‌اوت نمایشی (مانند `quran-ayah`، `quran`، `quote` و...).
3. **Ayah Note Folder:** انتخاب پوشه پیش‌فرض برای ذخیره‌سازی یادداشت‌های آیات (با راهنمای هوشمند پوشه‌ها).
4. **Ayah Note Path Pattern:** انتخاب ساختار نام فایل‌ها (انگلیسی/عربی و استفاده از اسلش یا خط تیره).
5. **Ayah Note Tags:** برچسب‌های متادیتا که به صورت خودکار به Frontmatter افزوده می‌شوند.
6. **Link to Surah:** اضافه کردن لینک سوره مربوطه در یادداشت آیه.
