# V28 — پرداخت idempotent و اعلان سفارش

اضافه شد:
- جلوگیری از پردازش دوباره callback یک تراکنش در لایه application
- abstraction اعلان وضعیت سفارش با SMS
- طراحی رویدادهای بعد از پرداخت

در Production باید idempotency key نیز در دیتابیس با UNIQUE constraint ذخیره شود تا حتی در چند instance سرور هم duplicate payment پردازش نشود.
