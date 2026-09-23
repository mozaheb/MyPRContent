# Persian AI Content Reasoning Protocol

Status: Canonical
Version: 1.3
Effective: 2026-09-23

## هدف

این سند فرآیند تولید MyPRContent توسط هوش مصنوعی را استاندارد می‌کند.

این پروتکل کیفیت تصمیم و خروجی را تعریف می‌کند؛ نه افشای استدلال داخلی مدل.

## اصل پایه

AI جایگزین یوسف نیست.

AI باید:
- دانش را سازمان دهد.
- Evidence را پیدا کند.
- تضاد را روشن کند.
- گزینه‌های خلاقانه بسازد.
- خروجی را برای رسانه بهینه کند.

POV نهایی باید با تجربه، داده و جهان‌بینی یوسف سازگار باشد.

## Source Resolution

پیش از تولید محتوای مهم:

۱. CANONICAL-HEAD.json
۲. ssot/MANIFEST.json
۳. اسناد Canonical مرتبط
۴. محتوای منتشرشده معتبر
۵. داده داخلی مجاز
۶. منابع عمومی تازه
۷. Trend Layer

Trend هرگز بر Core Strategy اولویت ندارد.


## Persian Language Baseline — Mandatory

برای هر خروجی فارسی، پیش از Draft باید `language/persian-writing-external-baseline.md` اعمال شود.

حداقل مسیر اجباری:
1. تشخیص Register بر اساس artifact و audience.
2. اعمال Voice داخلی MyPRContent.
3. خواندن و اعمال قواعد نسخه پین‌شده upstream برای `SKILL.md`، `references/writing-style.md` و `references/orthography.md`.
4. اجرای Naturalness و Orthography pass پیش از تحویل.
5. در خروجی فایل‌محور، اعمال reference مرتبط با RTL/format از همان نسخه پین‌شده.

Skip کردن این مرحله بدون دلیل مستند مجاز نیست.

## Decision Lens

موضوع از شش زاویه بررسی شود:

### Signal
چه چیزی تغییر کرده است؟

### Business Impact
این تغییر چه اثر اقتصادی یا مدیریتی دارد؟

### System
مسئله با سیستم حل می‌شود یا فقط تاکتیک است؟

### Risk
بزرگ‌ترین ریسک تصمیم چیست؟

### Experiment
کم‌هزینه‌ترین آزمون معتبر چیست؟

### Scale
اگر جواب داد، چگونه تکرار و مقیاس می‌شود؟

## Evidence Hierarchy

ترتیب اعتبار:

۱. داده داخلی تأییدشده و قابل انتشار
۲. تجربه مستقیم یوسف یا تیم
۳. منبع رسمی و تازه
۴. پژوهش معتبر
۵. Case Study شخص ثالث
۶. مشاهده بازار
۷. استنباط
۸. پیش‌بینی

سطح ۷ و ۸ باید صریحاً تحلیل یا پیش‌بینی معرفی شوند.

## Content Distillation

پیش از نوشتن یک جمله مرکزی ساخته شود:

**این محتوا دقیقاً چه چیزی را در ذهن یا تصمیم مخاطب تغییر می‌دهد؟**

اگر بیش از یک ایده اصلی وجود دارد، محتوا تقسیم شود.

## Narrative & Retention Skill — Conditional

برای طراحی Hook، Retention، Progressive Disclosure یا روایت، از `ai/skills/story-hook-content-engine/SKILL.md` نسخه ثبت‌شده در SSOT استفاده شود.

این Skill «Storytelling اجباری» نیست.

پیش از فعال‌سازی باید این موارد حل شوند:
1. Content Job
2. Core Claim
3. Evidence Token
4. Signature Series
5. Channel
6. Confidentiality

سپس Story Fit Test اجرا شود و یکی از سه حالت انتخاب شود:
- Narrative-first
- Hybrid
- Direct-first

منابع پشتیبان Skill:
- `ai/skills/story-hook-content-engine/references/routing-and-channel-profiles.md`
- `ai/skills/story-hook-content-engine/references/hook-pattern-library.md`
- `ai/skills/story-hook-content-engine/references/quality-gate.md`

ترتیب تقدم:
**Strategy → Evidence → Confidentiality → Canonical Terminology → Persian Language Baseline → Channel Constraints → Signature Series → Story Hook Skill → Trend Tactics**

قواعد اجباری:
- Evidence قبل از Storytelling حل شود.
- تجربه، نقل‌قول، عدد و Case ساخته نشود.
- Storytelling حق تأخیر غیرضروری در پاسخ مدیریتی را ندارد.
- در محتوای AI Search یا Citation-oriented، Answer-first حفظ شود.
- Mechanism نمونه خارجی منتقل شود؛ نه ظاهر، جمله یا شخصیت Creator.
- Skill باید Quality Gate حداقل 90/100 را بدون Hard Fail پاس کند.
- اگر Evidence ناکافی است، وضعیت `Evidence Needed` حفظ شود و ready-to-publish اعلام نشود.

این Skill پس از Content Distillation و پیش از Draft Protocol اجرا می‌شود.

## Contrarian Test

بررسی شود:
- باور رایج چیست؟
- آیا Evidence برای زاویه متفاوت وجود دارد؟
- آیا تفاوت واقعی است یا برای جنجال ساخته شده است؟

Contrarian بدون Evidence ممنوع است.

## Novelty Test

پرسش اجباری:

**آیا یک کپی‌رایتر عمومی با یک Prompt ساده می‌تواند همین متن را تولید کند؟**

اگر بله، حداقل یکی اضافه شود:
- داده
- تجربه
- تصمیم واقعی
- پیش‌بینی ثبت‌شده
- آزمایش
- زاویه فکری اختصاصی

## Trend Hijack Filter

ترند فقط وقتی استفاده شود که حداقل ۳ شرط را داشته باشد:

۱. با Business Growth Architecture مرتبط باشد.
۲. یوسف POV اختصاصی داشته باشد.
۳. اثر تصمیمی برای مخاطب داشته باشد.
۴. Evidence یا تجربه قابل افزودن باشد.
۵. عمر محتوا از موج اولیه بیشتر باشد.

اگر فقط «داغ» است، وارد MyPRContent نشود.

## Headline Generation Protocol

برای محتوای مهم حداقل ۱۲ تیتر داخلی تولید شود.

تیترها از Archetypeهای مختلف باشند.

امتیازدهی:

| معیار | وزن |
|---|---:|
| وضوح | ۲۰ |
| کنجکاوی | ۱۵ |
| تمایز | ۱۵ |
| اعتبار و Evidence | ۱۵ |
| تناسب با برند | ۱۵ |
| طبیعی‌بودن فارسی | ۱۰ |
| قابلیت استخراج AI | ۵ |
| کنترل Clickbait | ۵ |

فقط بهترین گزینه‌ها به کاربر نشان داده شوند.

## Draft Protocol

ساختار پیش‌فرض:

**Hook → Tension → Evidence → Reframe → Decision**

پیش از نوشتن:
### Pass 0 — Register
Register بر اساس نوع artifact، مخاطب و کانال تعیین و در کل خروجی ثابت نگه داشته شود.

سپس پنج Pass انجام شود:

### Pass 1 — Persian Naturalness
ترجمه‌زدگی، عبارت ماشینی، نثر اداری مصنوعی و AI-tellهای شناخته‌شده بر اساس Persian Writing Baseline حذف شوند.

### Pass 2 — Compression
تکرار و مقدمه غیرضروری حذف شود.

### Pass 3 — Evidence
ادعای مهم بررسی شود.

### Pass 4 — Extraction
پاراگراف مهم مستقل و قابل نقل شود.

### Pass 5 — Orthography
نیم‌فاصله، ی/ک فارسی، اعداد، punctuation، هکسره و یکدستی رسم‌الخط بر اساس Persian Writing Baseline کنترل شوند.

## Risk Review

پیش از انتشار بررسی شود:
- محرمانگی
- داده شخصی
- ادعای حساس
- آمار بی‌منبع
- افشای مزیت رقابتی
- پیش‌بینی قطعی
- Context ناقص

## Learning Loop

پس از انتشار فقط Reach بررسی نشود.

بررسی شود:
- کدام Hook پاسخ باکیفیت ساخت؟
- کدام جمله Save یا Share شد؟
- چه نوع مخاطبی واکنش داد؟
- کدام موضوع DM یا Opportunity ساخت؟
- آیا محتوا در AI Search دیده شد؟
- چه الگویی باید وارد Pattern Library شود؟

نتیجه به Trend Layer برگردد.
