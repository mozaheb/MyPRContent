---
name: story-hook-content-engine
version: 2.0
status: canonical-operational
effective: 2026-09-23
description: موتور تصمیم‌گیری برای Hook، روایت، Retention و Progressive Disclosure در MyPRContent. ابتدا تشخیص می‌دهد روایت مناسب است یا نه؛ سپس بر اساس Strategy، Evidence، Signature Series، Channel و Quality Gate ساختار مناسب را می‌سازد یا بازنویسی می‌کند.
---

# Story Hook Content Engine — v2.0

## مأموریت

این Skill برای «داستانی‌کردن همه محتواها» ساخته نشده است.

وظیفه آن این است که بهترین معماری توجه و روایت را برای هر محتوا انتخاب کند.

هدف نهایی:

**توقف درست → فهم سریع → کشش معتبر → شاهد → تغییر زاویه دید → تصمیم**

Storytelling فقط وقتی استفاده می‌شود که فهم، اعتبار یا ماندگاری محتوا را بهتر کند.

## جایگاه در SSOT

این Skill زیرمجموعه Strategy نیست و حق تغییر Strategy را ندارد.

ترتیب تقدم:

1. دستور صریح کاربر
2. Strategy و Brand Core
3. Evidence و Confidentiality
4. Canonical Terminology
5. Persian Voice و Writing Standards
6. Channel Constraints
7. Signature Series
8. این Skill
9. Trend و Hook Tactics

منابع اجباری پیش از اجرای محتوای مهم:

- `CANONICAL-HEAD.json`
- `ssot/MANIFEST.json`
- `strategy/master-strategy-v2.md`
- `strategy/content-season-01.md` در محتوای Season 01
- `strategy/signature-series.md`
- `strategy/channel-system.md`
- `governance/content-rules.md`
- `governance/confidentiality.md`
- `language/persian-voice-and-tone.md`
- `language/persian-writing-standard.md`
- `language/persian-writing-external-baseline.md`
- `templates/persian-content-output-contract.md`

منابع داخلی این Skill:

- `references/routing-and-channel-profiles.md`
- `references/hook-pattern-library.md`
- `references/quality-gate.md`

## North Star

محتوا باید به جای «جلب توجه صرف»، مرجعیت فکری بسازد.

هر خروجی باید حداقل یکی از این آثار را ایجاد کند:

- سیگنال را زودتر نشان دهد.
- تصمیم را روشن‌تر کند.
- مسئله را به سیستم تبدیل کند.
- ریسک را بهتر صورت‌بندی کند.
- یک آزمایش معتبر پیشنهاد دهد.
- امکان مقیاس‌دادن را روشن کند.

مدل پایه MyPRContent:

**Signal → Decision → System → Experiment → Scale**

## Input Contract

پیش از تولید، این فیلدها را حل کن.

### Required

- **content_goal:** چه تغییر ذهنی یا تصمیمی باید ایجاد شود؟
- **audience:** مخاطب دقیق کیست؟
- **channel:** کجا منتشر می‌شود؟
- **core_claim:** یک ادعای مرکزی چیست؟
- **evidence_token:** شاهد چیست؟
- **evidence_source:** شاهد از کجا آمده است؟
- **confidentiality:** Public / Selective / Private
- **series:** RADAR / DECISION / GROWTH / DATA / RETHINK / LAB یا None
- **desired_action:** مخاطب بعد از محتوا چه چیزی را باید متفاوت ببیند یا انجام دهد؟

### Contextual

- content_id
- funnel_stage
- format
- cover_required
- publication_status
- recent_hook_patterns
- recent_channel_mix
- available_measurement

اگر Content ID در SSOT وجود دارد، داده را از Registry و Queue بازیابی کن.

اگر Evidence وجود ندارد، آن را نساز.

خروجی را با وضعیت **Evidence Needed** نگه دار.

## Step 0 — Content Job

ابتدا Job محتوا را مشخص کن.

یکی از این نقش‌ها انتخاب شود:

- **POV:** تغییر زاویه دید
- **Evidence:** اثبات یک Claim
- **Decision:** نشان‌دادن منطق تصمیم
- **Operator/Human:** نشان‌دادن انسان پشت تصمیم
- **Future Signal:** تفسیر یک تغییر آینده
- **Data-to-Decision:** تبدیل داده به اقدام
- **Case/Lab:** آزمایش و Learning
- **Synthesis:** جمع‌بندی چند شاهد برای ساخت Framework

هر محتوا یک Job اصلی دارد.

Job دوم فقط در صورت ضرورت اضافه شود.

## Step 1 — Story Fit Test

پیش از Storytelling، این پنج سؤال را بررسی کن:

1. آیا صحنه، رخداد، تصمیم یا تغییر واقعی وجود دارد؟
2. آیا روایت فهم مسئله را بهتر می‌کند؟
3. آیا Evidence داخل روایت قابل نمایش است؟
4. آیا Progressive Disclosure ارزش ایجاد می‌کند؟
5. آیا روایت باعث تأخیر غیرضروری در پاسخ نمی‌شود؟

### نتیجه

- 4–5 پاسخ مثبت: **Narrative-first**
- 2–3 پاسخ مثبت: **Hybrid**
- 0–1 پاسخ مثبت: **Direct-first**

اگر مخاطب پاسخ سریع و تصمیمی می‌خواهد، Direct-first اولویت دارد.

اگر محتوا Citation-oriented یا AI Search-oriented است، Answer-first حفظ شود.

## Step 2 — Signature Series Routing

ساختار سری بر Hook مقدم است.

### RADAR

**Signal → Why it matters → Winners/Losers → Decision now**

قلاب باید تغییر را روشن کند، نه آینده را هیجان‌زده نشان دهد.

### DECISION

**مسئله → گزینه‌ها → ریسک → تصمیم → نتیجه**

قلاب از trade-off، هزینه تأخیر یا تصمیم خلاف انتظار ساخته شود.

### GROWTH

**Constraint → Lever → System → Experiment → Scale**

قلاب از اصطکاک، گلوگاه یا رفتار عادی‌شده ساخته شود.

### DATA

**Chart/Delta → Meaning → Decision**

قلاب از تغییر مهم ساخته شود، نه صرفاً عدد بزرگ.

### RETHINK

**باور قبلی → شواهد جدید → خطا → اصلاح**

قلاب باید تغییر باور واقعی را نشان دهد.

### LAB

**Hypothesis → Build/Test → Evidence → Learning**

قلاب از آزمایش، نتیجه یا شکست معتبر ساخته شود.

## Step 3 — Hook Selection

Hook باید سه کار انجام دهد:

**فهم سریع + تنش ذهنی + وعده معتبر**

حداقل دو جزء داشته باشد:

- Context تخصصی
- تضاد یا ناهنجاری
- پیامد مدیریتی
- Evidence signal
- Open Loop
- تصمیم یا trade-off
- تغییر باور

Hook نباید Context را آن‌قدر حذف کند که فریب ایجاد شود.

برای انتخاب خانواده Hook، از `references/hook-pattern-library.md` استفاده کن.

## Step 4 — Retention Architecture

Retention با «ابهام مصنوعی» ساخته نمی‌شود.

هر بخش باید یکی از این کارها را انجام دهد:

- سؤال قبلی را پاسخ دهد.
- شاهد تازه بدهد.
- زاویه را عوض کند.
- پیامد را روشن کند.
- تصمیم را نزدیک‌تر کند.

### Narrative-first

**Hook → Scene → Anomaly → Evidence → Re-hook → Reveal → Reframe → Decision**

### Hybrid

**Hook → Direct Claim → Scene/Evidence → Reframe → Decision**

### Direct-first

**Answer/Claim → Evidence → Implication → Decision**

در Direct-first نتیجه را بی‌دلیل پنهان نکن.

## Step 5 — Scene Engine

فقط وقتی Story Fit تأیید شده است، Scene بساز.

صحنه باید واقعی یا صریحاً فرضی باشد.

اجزای مفید:

- نقش مشخص
- مکان یا Context
- دیالوگ کوتاه
- رفتار قابل مشاهده
- عدد
- صفحه، نمودار، تیکت، پیام یا شیء
- لحظه تصمیم
- پیامد

از «جزئیات تزئینی» که Evidence را تقویت نمی‌کنند، پرهیز کن.

## Step 6 — Progressive Disclosure

هر Reveal باید ارزش شناختی داشته باشد.

ترتیب پیشنهادی:

1. اتفاق یا Claim
2. ناهنجاری
3. شاهد
4. تفسیر
5. سؤال مهم‌تر
6. Reveal
7. Reframe
8. Decision

Open Loop باید در همان محتوا بسته شود.

ابهام unresolved برای افزایش Engagement ممنوع است.

## Step 7 — B2B Tension Sources

در B2B از هیجان مصنوعی استفاده نکن.

Tension را از این منابع بگیر:

- اصطکاک عادی‌شده
- هزینه پنهان
- فاصله داده تا تصمیم
- کار دستی باقی‌مانده پس از نرم‌افزار
- وابستگی به حافظه فرد
- Hand-off
- تصمیم دیرهنگام
- trade-off
- شکاف ابزار و فرایند
- رفتار کاربر که فرض را نقض می‌کند
- فرصت ازدست‌رفته
- ریسک عدم اقدام

## Step 8 — Anti-Copy Moat

پیش از Draft پاسخ بده:

**چه چیزی در این محتوا بدون تجربه، داده، تصمیم یا جهان‌بینی یوسف قابل تولید نیست؟**

حداقل یک Moat باید وجود داشته باشد:

- Data Moat
- Operator Moat
- Decision Moat
- Prediction Moat
- Thinking Moat

اگر هیچ Moat وجود ندارد، Draft نهایی تولید نکن.

ابتدا Evidence یا POV لازم را مشخص کن.

## Step 9 — Channel Adaptation

یک Master Claim می‌تواند چند اجرای بومی داشته باشد.

Copy/Paste میان کانال‌ها ممنوع است.

قواعد کامل در `references/routing-and-channel-profiles.md` است.

Fact، Position، عدد، Entity، تاریخ و سطح قطعیت بین کانال‌ها تغییر نمی‌کنند.

## Step 10 — Headline and Cover

Headline، Cover Headline و Opening Hook یک چیز نیستند.

برای محتوای مهم:

1. حداقل 12 تیتر داخلی تولید کن.
2. تنوع خانواده تیتر را حفظ کن.
3. بهترین 6 گزینه را طبق Output Contract انتخاب کن.
4. پیشنهاد اصلی را فقط بر اساس تطابق با Claim انتخاب کن.

Cover:

- 5 تا 9 واژه
- یک Claim
- بدون CTA فروش
- بدون Clickbait تصویری
- مطابق `design/cover-system.md`

## Step 11 — CTA

CTA فقط وقتی اضافه شود که نقش مشخص داشته باشد.

انواع مناسب:

- سؤال تصمیمی
- دعوت به تجربه واقعی
- اقدام عملی
- درخواست مثال مشخص
- دعوت به مقایسه یک تصمیم

این موارد ممنوع‌اند:

- «نظر شما چیست؟» به‌عنوان CTA عمومی
- Engagement bait
- سؤال بدون ارتباط با Claim

## Step 12 — Evidence and Truth Boundary

بین این چهار نوع جمله تفکیک کن:

- **Fact**
- **Interpretation**
- **Prediction**
- **Claim**

Prediction باید تاریخ‌دار یا صریحاً پیش‌بینی معرفی شود.

این موارد Hard Fail هستند:

- تجربه جعلی
- نقل‌قول جعلی
- عدد بی‌منبع
- Case Study ساختگی
- نسبت‌دادن انگیزه بدون شاهد
- حذف Context برای جذابیت
- ادعای بزرگ‌تر از Evidence

## Step 13 — Confidentiality

قبل از استفاده از تجربه واقعی بررسی کن:

- داده مشتری قابل شناسایی نباشد.
- قرارداد و قیمت اختصاصی منتشر نشود.
- اسرار تجاری افشا نشود.
- Playbook رقابتی لو نرود.
- اطلاعات کارکنان بدون مجوز استفاده نشود.
- Product Roadmap محرمانه منتشر نشود.

در تردید، Detail را حذف یا Aggregate کن.

## Step 14 — Persian Execution

در فارسی این منابع اجباری‌اند:

- `language/persian-voice-and-tone.md`
- `language/persian-writing-standard.md`
- `language/persian-writing-external-baseline.md`
- `language/persian-canonical-lexicon.md`

قواعد حداقلی:

- فارسی معیار، طبیعی و حرفه‌ای
- جمله ترجیحاً حداکثر 20 واژه
- فعل تا حد امکان در پایان
- پاراگراف یک‌وظیفه‌ای
- نیم‌فاصله صحیح
- ی و ک فارسی
- بدون نثر ترجمه‌زده
- بدون AI-tell
- بدون واژه انگلیسی نمایشی
- بدون ایموجی در حالت پیش‌فرض MyPRContent

## Step 15 — Output Contract

پیش‌فرض = Mode M.

خروجی نهایی باید با `templates/persian-content-output-contract.md` سازگار باشد.

حداقل شامل:

1. Strategic Intent
2. Headline Set
3. Cover Copy در صورت نیاز
4. Opening Options
5. Main Copy
6. CTA Options
7. Evidence & Risk Note
8. Channel Adaptation در صورت درخواست
9. Machine Metadata
10. AI Extraction Block برای محتوای عمیق

اگر کاربر فقط متن نهایی خواسته است، اجزای تحلیلی را نمایش نده.

## Step 16 — Quality Gate

پیش از تحویل، `references/quality-gate.md` را اجرا کن.

قواعد اصلی:

- امتیاز هدف: **90/100 یا بیشتر**
- Hard Fail مستقل از امتیاز است.
- 80–89: بازنویسی اجباری
- کمتر از 80: ساختار باید عوض شود.
- Evidence ضعیف با نثر قوی جبران نمی‌شود.

## Step 17 — Self-Correction Loop

حداکثر سه Pass انجام بده.

### Pass 1 — Architecture

بررسی:

- Job
- Series
- Story Fit
- Channel
- Claim
- Evidence

### Pass 2 — Retention

بررسی:

- Hook
- Progressive Disclosure
- Re-hook
- Payoff
- حذف بخش‌های بدون وظیفه

### Pass 3 — Trust

بررسی:

- Fact/Interpretation/Prediction
- Confidentiality
- Natural Persian
- Anti-copy
- CTA
- Metadata

اگر پس از سه Pass هنوز زیر Gate است، آن را ready-to-publish اعلام نکن.

## Step 18 — Season Continuity

در Season 01 این قواعد اجباری‌اند:

- هیچ سه محتوای متوالی Hook pattern مشابه نداشته باشند.
- در هر بلوک 6 محتوا، حداکثر 2 تیتر پرسشی محدود باشد.
- هیچ پنج محتوای متوالی فقط Text Post نباشند.
- هر هفته حداقل یک Evidence-led asset وجود داشته باشد.
- Narrative Order بدون Evidence تغییر نکند.
- Core Strategy با یک پست تغییر نکند.

در صورت امکان، 3 تا 5 محتوای اخیر را پیش از انتخاب Hook بررسی کن.

## Step 19 — Post-Publication Learning

پس از انتشار، Hook فقط با Reach سنجیده نمی‌شود.

حداقل بررسی:

- Distribution
- Qualified comments
- Save/share
- Video retention یا Read depth
- Decision-maker response
- Qualified DM
- Profile/follower quality
- Opportunity signal
- Evidence type performance

Learning را به یکی از این دسته‌ها ثبت کن:

- Hook
- Audience
- Format
- Topic
- CTA
- Timing

یک پست برای تغییر Strategy کافی نیست.

## حالت تحلیل نمونه خارجی

اگر ویدئو، پست یا Creator نمونه داده شد:

1. Mechanism را استخراج کن.
2. Evidence و Context آن نمونه را جدا کن.
3. Platform-specific tactic را از Structural Pattern جدا کن.
4. Transferability را بسنج.
5. چیزی را که فقط به شخصیت Creator وابسته است حذف کن.
6. فقط Pattern قابل انتقال را وارد MyPRContent کن.

قاعده:

**Mechanism را منتقل کن؛ ظاهر، جمله و شخصیت را تقلید نکن.**

## اصل نهایی

Hook هدف نیست.

Retention هدف نیست.

هدف این است که مخاطب درست، یک فکر مهم را تا رسیدن به Evidence و Decision دنبال کند.

**Attention باید به Authority و سپس Opportunity کمک کند.**
