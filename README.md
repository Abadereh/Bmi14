# Bmi14 APK Builder

این repo برای ساخت APK برنامه جستجوی کد شعبه بانک ملی از روی فایل ZIP آماده شده است.

## روش استفاده سریع

1. فایل `bmi-v13.zip` را در ریشه همین repo آپلود کن.
2. بعد از commit، وارد تب **Actions** شو.
3. workflow با نام **Build Release APK from uploaded ZIP** را اجرا یا نتیجه اجرای خودکار را باز کن.
4. خروجی از بخش Artifacts با نام `bmi14-release-apk` قابل دانلود است.

## نکته مهم

این repo طوری آماده شده که نیازی نیست فایل‌های داخل ZIP را دونه‌دونه آپلود کنی. فقط خود فایل ZIP را در ریشه repo بگذار.

## Secrets لازم برای خروجی release مناسب بازار

در مسیر زیر بساز:

```text
Settings > Secrets and variables > Actions > New repository secret
```

Secretهای لازم:

```text
SIGNING_KEYSTORE_BASE64
SIGNING_STORE_PASSWORD
SIGNING_KEY_ALIAS
SIGNING_KEY_PASSWORD
BAZAAR_RSA_PUBLIC_KEY
BAZAAR_PURCHASE_PRODUCT_ID
```

## مدل پرداخت

نسخه فعلی برای خرید یک‌باره آماده شده است، نه اشتراک ماهانه یا سالانه.

شناسه پیشنهادی محصول:

```text
bmi_branches_lifetime
```
