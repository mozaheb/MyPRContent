# Persian Content Output Contract

Status: Canonical
Version: 1.1
Effective: 2026-09-22

## هدف

هر محتوای مهم MyPRContent باید قابل انتخاب، انتشار، سنجش و یادگیری باشد.


## Mandatory Language Preflight

هر خروجی فارسی این Contract فقط زمانی کامل محسوب می‌شود که `language/persian-writing-external-baseline.md` را پاس کرده باشد.

پیش از تحویل یا تغییر وضعیت به `ready-to-publish`:
- Register باید تعیین و در متن ثابت باشد.
- Naturalness pass و حذف AI-tellهای مرتبط انجام شده باشد.
- Orthography pass انجام شده باشد.
- در خروجی فایل‌محور، RTL و قواعد فرمت فارسی نیز بررسی شده باشد.

این شرط با کوتاه‌بودن خروجی یا انتخاب Mode S حذف نمی‌شود.

## Default Output

مگر اینکه درخواست دیگری داده شود، خروجی شامل این بخش‌ها باشد:

### 1. Strategic Intent
در یک یا دو جمله:
- هدف
- مخاطب
- تغییر ذهنی یا رفتاری مطلوب

### 2. Headline Set
۶ گزینه:
- A شفاف
- B تضاد
- C پرسشی
- D داده
- E تصمیم
- F آینده

یک گزینه با عنوان **پیشنهاد اصلی** مشخص شود.

### 3. Cover Copy
- Series ID
- تیتر ۵ تا ۹ واژه
- Evidence Line اختیاری

### 4. Opening Options
سه Hook:
- مستقیم
- روایی
- جسور

### 5. Main Copy
نسخه اصلی آماده انتشار.

### 6. CTA Options
سه مدل:
- پرسش تصمیمی
- دعوت به تجربه
- اقدام عملی

CTA عمومی «نظر شما چیست؟» استفاده نشود.

### 7. Evidence & Risk Note
در صورت نیاز:
- Source
- Data caveat
- Prediction label
- Confidentiality risk

### 8. Channel Adaptations
فقط برای کانال‌های خواسته‌شده.

## Output Modes

### Mode S — Fast
۳ تیتر + ۱ متن کوتاه + ۱ CTA

### Mode M — Standard
۶ تیتر + Cover + ۳ Hook + متن اصلی + ۳ CTA

### Mode L — Campaign
۱۲+ تیتر اولیه، Master Asset، نسخه‌های رسانه‌ای، ویدئو، Carousel، Cover، CTA، Metadata و Measurement Plan

پیش‌فرض MyPRContent = Mode M.

## Machine Metadata

هر Master Content باید قابلیت ذخیره این Metadata را داشته باشد:

- id
- date
- language
- series
- channel
- audience
- funnel_stage
- core_claim
- evidence_type
- evidence_source
- prediction
- confidentiality
- canonical_terms
- cover_template
- cta_type
- status

نمونه شناسه:
GROWTH-012-fa-v3

## AI Extraction Block

برای محتوای عمیق، نسخه Canonical یک Answer Block داشته باشد:

**سؤال اصلی:**  
...

**پاسخ کوتاه:**  
...

**دلیل:**  
...

**اقدام پیشنهادی:**  
...

این Block الزاماً عیناً در شبکه اجتماعی منتشر نمی‌شود.

## Versioning

هر بازنویسی اساسی Revision جدید بگیرد.

نسخه منتشرشده باید قابل ردیابی باشد.
