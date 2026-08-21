# V22 — Session و Production Security

اضافه شد:
- Session token با TTL هفت‌روزه
- logout و revoke
- middleware نقش‌ها
- جلوگیری از صدور session مدیر از endpoint عمومی

قبل از انتشار واقعی:
- Session باید در دیتابیس/Redis persistent شود.
- cookie امن HttpOnly/Secure/SameSite برای browser ترجیح دارد.
- OTP verification باید مستقیماً پس از verify، session مشتری را ایجاد کند.
- Admin باید با حساب و credential مستقل provision شود.
- secrets فقط در environment/server secret store.
