<div dir="rtl">

# 🤖 AI Chat Pro — چت‌بات هوش مصنوعی فارسی

یه اپلیکیشن چت هوش مصنوعی رایگان با قابلیت تولید و ویرایش تصویر. بدون نیاز به نصب، فقط با یه فایل HTML کار میکنه.

</div>

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen?style=for-the-badge)](https://niksiratforex-ux.github.io/ai-image-generator/)
![HTML5](https://img.shields.io/badge/HTML5-single%20file-orange?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)

---

## ✨ ویژگی‌ها

### 💬 چت هوش مصنوعی
- پشتیبانی از چندین provider: **Gemini**، **OpenRouter**، **Groq**، **Pollinations**
- چت چندتبی — چند مکالمه همزمان
- پرامپت‌های سریع (ترجمه، خلاصه، توضیح، تحلیل و...)
- ذخیره خودکار تاریخچه چت در مرورگر

### 🎨 تولید تصویر
- تولید تصویر از متن با **Pollinations** (رایگان، بدون API key)
- مدل‌های متنوع: FLUX، FLUX Anime، FLUX 3D، Turbo

### ✏️ ویرایش تصویر
- عکس بفرست + پرامپت بنویس = عکس ویرایش‌شده
- با **Pollinations Kontext** (رایگان با API key)
- با **Gemini** multimodal (رایگان با API key)
- مدل‌های ویرایش: Kontext، NanoBanana، Seedream

### 📱 رابط کاربری
- طراحی **RTL فارسی** با فونت Vazirmatn
- تم تاریک و روشن
- کاملاً **responsive** — موبایل، تبلت، دسکتاپ
- سوییچ سریع بین provider‌ها
- ضمیمه عکس با 📎، Ctrl+V، Drag & Drop
- پنل راهنمای کامل

### 📤 خروجی
- خروجی TXT و JSON از چت‌ها
- کپی پیام با یه کلیک
- لایت‌باکس تصاویر

---

## 🚀 راه‌اندازی

### استفاده ساده (GitHub Pages)

فقط فایل `ai-chat-pro.html` رو توی ریپازیتوری آپلود کن و GitHub Pages رو فعال کن.

### استفاده محلی

```bash
# با Python
python3 -m http.server 8080

# یا با Node.js
npx serve .

# بعد توی مرورگر باز کن:
# http://localhost:8080/ai-chat-pro.html
```

> ⚠️ فایل رو مستقیم با `file://` باز نکنید — بعضی API‌ها CORS بلاک میکنن.

---

## 🔑 API Key‌ها

| سرویس | نیاز به Key | دریافت | رایگان |
|--------|:----------:|--------|:-----:|
| **Gemini** | ✅ بله | [aistudio.google.com](https://aistudio.google.com/app/apikey) | ✅ کاملاً رایگان |
| **OpenRouter** | ✅ بله | [openrouter.ai](https://openrouter.ai/keys) | ✅ مدل‌های رایگان |
| **Groq** | ✅ بله | [console.groq.com](https://console.groq.com/keys) | ✅ رایگان |
| **Pollinations** | اختیاری | [enter.pollinations.ai](https://enter.pollinations.ai/keys) | ✅ تولید رایگان |

> 💡 **Pollinations** بدون key هم برای تولید تصویر کار میکنه. برای ویرایش تصویر، key لازمه.

---

## 📖 راهنمای سریع

### تولید تصویر
1. Provider رو روی **🎨 Pollinations** بذار
2. پرامپت بنویس: `یک گربه با عینک آفتابی روی موتور`
3. ارسال بزن ✅

### ویرایش تصویر
1. عکس رو ضمیمه کن (📎 یا Ctrl+V)
2. Provider رو **🎨 Pollinations** کن
3. مدل **kontext** رو انتخاب کن
4. پرامپت ویرایش رو بنویس: `پس‌زمینه رو ساحل کن`
5. ارسال بزن ✅

### چت متنی
1. Provider رو روی **Gemini** یا **OpenRouter** بذار
2. API key رو توی تنظیمات وارد کن
3. پیامت رو بنویس و ارسال کن

---

## 🛠️ ساختار فایل

```
ai-chat-pro.html    ← فایل اصلی (همه چیز تو یه فایل)
```

- **HTML** + **CSS** + **JavaScript** — بدون وابستگی خارجی
- فونت Vazirmatn از Google Fonts
- ذخیره‌سازی با `localStorage`

---

## 📸 اسکرین‌شات

<div align="center">

| تم تاریک | تم روشن |
|:---------:|:-------:|
| 🌙 Dark Mode | ☀️ Light Mode |

</div>

---

## 🔧 تنظیمات

از دکمه ⚙️ میتونی:

- **API Key** هر سرویس رو وارد کنی
- **مدل** مورد نظر رو انتخاب کنی
- **پرامپت سیستم** رو تغییر بدی
- **دما (Temperature)** رو تنظیم کنی
- **حداکثر توکن** رو مشخص کنی
- **اتصال** رو تست کنی
- **خروجی** بگیری

---

## 📋 مدل‌های پشتیبانی شده

### Gemini (رایگان)
| مدل | ویرایش تصویر | توضیح |
|-----|:----------:|-------|
| `gemini-2.5-flash` | ✅ | سریع و رایگان |
| `gemini-2.5-pro` | ✅ | کیفیت بالاتر |
| `gemini-3-pro-image-preview` | ✅ | جدیدترین |
| `gemini-3.1-flash-image` | ✅ | Nano Banana 2 |

### Pollinations (رایگان)
| مدل | تولید | ویرایش | توضیح |
|-----|:-----:|:-----:|-------|
| `flux` | ✅ | ✅ | عمومی |
| `flux-realism` | ✅ | - | واقع‌گرایانه |
| `flux-anime` | ✅ | - | انیمه |
| `flux-3d` | ✅ | - | سه‌بعدی |
| `turbo` | ✅ | - | سریع |
| `kontext` | - | ✅ | ویرایش عمومی |
| `nanobanana-2` | - | ✅ | ویرایش با کیفیت |
| `seedream` | - | ✅ | ویرایش خلاقانه |

### OpenRouter
| مدل | رایگان |
|-----|:-----:|
| `google/gemini-2.5-flash` | ✅ |
| `deepseek/deepseek-chat-v3.1` | ✅ |
| `anthropic/claude-sonnet-4` | ❌ |
| `openai/gpt-oss-20b:free` | ✅ |

### Groq
| مدل | رایگان |
|-----|:-----:|
| `llama-3.3-70b-versatile` | ✅ |
| `llama-3.1-8b-instant` | ✅ |
| `mixtral-8x7b-32768` | ✅ |

---

## 🤝 مشارکت

PR و Issue خوش آمدید!

1. ریپازیتوری رو fork کنید
2. Branch بسازید: `git checkout -b feature/amazing-feature`
3. Commit بزنید: `git commit -m 'Add amazing feature'`
4. Push کنید: `git push origin feature/amazing-feature`
5. PR بسازید

---

## 📄 لایسنس

MIT License — استفاده آزاد

---

<div dir="rtl">

## 🙏 تشکر

- [Pollinations.ai](https://pollinations.ai) — API رایگان تصویرسازی
- [Google AI Studio](https://aistudio.google.com) — API رایگان Gemini
- [Vazirmatn Font](https://github.com/rastikerdar/vazirmatn) — فونت فارسی
- [OpenRouter](https://openrouter.ai) — دسترسی به مدل‌های متنوع

</div>
