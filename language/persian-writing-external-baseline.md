# Persian Writing External Baseline

Status: Canonical  
Version: 1.0  
Effective: 2026-09-22

## Purpose

این سند وابستگی هنجاری MyPRContent به مرجع `ali2000hos/persian-writing` را ثبت و enforce می‌کند.

هدف این وابستگی، تضمین نثر فارسی روان، طبیعی، حرفه‌ای و از نظر رسم‌الخط و RTL صحیح است. این مرجع جایگزین Strategy، Voice، Evidence، Confidentiality یا Canonical Terminology پروژه نیست؛ فقط لایه زبان و ارائه فارسی را تکمیل می‌کند.

## Normative External Dependency

- Repository: https://github.com/ali2000hos/persian-writing
- Upstream version: 1.3.6
- Pinned commit: `35eb7a504f587e5baea4975476764f575773fa6b`
- Entry point: `SKILL.md`
- Local resilience snapshot: `vendor/persian-writing/v1.3.6/`
- Local self-contained knowledge: `vendor/persian-writing/v1.3.6/persian-writing-universal.md`
- Local mirrored source: `vendor/persian-writing/v1.3.6/source/`
- Always-required references for Persian prose:
  - `references/writing-style.md`
  - `references/orthography.md`
- License: MIT
- Scope: هر خروجی فارسی یا خروجی برای مخاطب فارسی‌زبان، شامل متن، ویرایش، ترجمه، کپشن، پست، مقاله، ایمیل، گزارش و اسناد RTL.

نسخه upstream جدید به‌صورت خودکار الزام‌آور نمی‌شود. ارتقا فقط پس از review و تغییر commit پین‌شده در SSOT مجاز است.

## Precedence

در صورت تعارض، ترتیب اولویت این است:

1. دستور صریح کاربر برای همان خروجی، تا جایی که با قواعد غیرقابل‌نقض پروژه تعارض نداشته باشد.
2. Strategy، Brand Core، Evidence، Confidentiality و Canonical Terminology در MyPRContent.
3. `language/persian-voice-and-tone.md` و `language/persian-writing-standard.md`.
4. این Baseline و نسخه پین‌شده `persian-writing` برای رجیستر، روانی نثر، رسم‌الخط و RTL.
5. قراردادهای عمومی یا پیش‌فرض مدل.

قواعد خارجی حق تغییر Positioning، ادعا، Fact/Prediction boundary، لحن اختصاصی برند یا واژگان Canonical را ندارند.

## Mandatory Workflow

برای هر خروجی فارسی:

1. **Register Detection** پیش از نوشتن انجام شود؛ نوع خروجی و مخاطب تعیین‌کننده است، نه لحن پیام درخواست.
2. **Brand Voice** از استاندارد داخلی MyPRContent اعمال شود.
3. **Naturalness Pass** انجام شود و نشانه‌های نثر اداری، ترجمه‌زده و ماشینی حذف شوند.
4. **Orthography Pass** شامل نیم‌فاصله، ی/ک فارسی، اعداد و نشانه‌گذاری صحیح انجام شود.
5. در خروجی‌های فایل‌محور، **RTL/Font/Layout Rules** مرتبط با فرمت اجرا شوند.
6. متن از Quality Gate داخلی عبور کند و فقط سپس ready-to-publish یا deliverable تلقی شود.

## Mandatory Naturalness Rules

حداقل این موارد باید کنترل شوند:

- رجیستر مناسب و ثابت در سراسر artifact.
- حذف عبارت‌های اداری و مصنوعی مانند «می‌باشد»، «لازم به ذکر است»، «در راستای» و مشابه آن، مگر ضرورت واقعی بافت.
- حذف آغازها و پایان‌های کلیشه‌ای مانند «در دنیای امروز» و «در نهایت می‌توان گفت».
- حذف ترجمه‌زدگی، تکرار مکانیکی connectorها و ریتم یکنواخت جمله‌ها.
- پرهیز از em dash در نثر فارسی.
- حفظ POV واحد و جلوگیری از جابه‌جایی بی‌دلیل میان «من»، «ما»، «شما» و بیان بی‌فاعل.
- تفکیک آموزش از تبلیغ و جلوگیری از ادعاهای بی‌پشتوانه.
- حفظ Fact / Interpretation / Prediction / Claim distinction.
- خواندن نهایی متن با معیار «آیا یک فارسی‌زبان حرفه‌ای واقعاً این‌طور می‌نویسد؟».

فهرست کامل الگوهای AI-tell و قواعد register از نسخه پین‌شده upstream پیروی می‌کند.

## Mandatory Orthography Rules

- نیم‌فاصله استاندارد در «می‌/نمی‌»، جمع‌ها، پسوندها و ترکیب‌های لازم.
- استفاده از «ی» و «ک» فارسی، نه نویسه‌های عربی.
- استفاده از اعداد فارسی در نثر فارسی؛ استثنا برای URL، کد، شناسه، نسخه و موارد ماشینی.
- استفاده از «،»، «؛»، «؟» و «گیومه» فارسی.
- کنترل هکسره و کسره اضافه.
- یکدستی فاصله‌گذاری و حذف فاصله‌های اضافی.
- عدم letter-spacing برای متن فارسی.

## Document & RTL Rule

هرگاه خروجی Word، PDF، PowerPoint، HTML، Excel یا تصویر فارسی است، علاوه بر مهارت/استاندارد فنی اصلی آن فرمت، مرجع پین‌شده `persian-writing` برای RTL، bidi، فونت و چیدمان فارسی نیز الزام‌آور است.

قواعد بصری برند MyPRContent یا درخواست صریح کاربر بر انتخاب رنگ و استایل مقدم‌اند؛ مرجع خارجی فقط مکانیک صحیح فارسی و RTL را تعیین می‌کند.

## Hard Fail

خروجی فارسی fail است اگر یکی از این موارد برقرار باشد:

- Register نامناسب یا ناپایدار باشد.
- نثر به‌وضوح ترجمه‌زده، اداریِ مصنوعی یا machine-like باشد.
- خطاهای آشکار نیم‌فاصله، ی/ک عربی، هکسره یا punctuation فارسی باقی مانده باشد.
- یک cluster از AI-tellهای شناخته‌شده بدون بازنویسی باقی مانده باشد.
- در سند فایل‌محور، RTL یا shaping فارسی شکسته باشد.
- قواعد این Baseline بدون دلیل مستند skip شده باشند.

## Review & Upgrade

- این dependency حداقل هم‌زمان با review دوره‌ای Language Core بررسی شود.
- تغییر upstream فقط پس از بررسی release notes و نمونه‌های regression وارد SSOT شود.
- هنگام ارتقا، `upstream version` و `pinned commit` در این سند، `CANONICAL-HEAD.json` و `ssot/MANIFEST.json` هماهنگ شوند.


## Local-First Resilience Rule

نسخه vendorشده داخل MyPRContent بخشی از SSOT است و برای تداوم دانش نگهداری می‌شود.

- برای اجرای روزمره، قواعد Canonical داخلی MyPRContent مقدم‌اند.
- برای جزئیات Persian Writing، ابتدا snapshot محلی نسخه پین‌شده قابل استفاده است.
- upstream فقط برای provenance، بررسی نسخه‌های جدید و upgrade review لازم است.
- اگر مخزن upstream حذف، خصوصی، جابه‌جا یا غیرقابل‌دسترسی شود، نسخه محلی بدون تغییر همچنان مرجع معتبر همان نسخه 1.3.6 است.
- هیچ حذف upstream نباید اجرای Language System را block کند.
