# Persian x-ui

پنل فارسی xray که از چند پروتکل و چند کاربر پشتیبانی می کند

# 🤵 برنامه نویس و توسعه دهنده
ابراهیم شفیعی 
# امکانات 

- پشتیبانی از زبان فارسی
- بدون هیچ گونه جاسوس افرازی
- نظارت بر وضعیت سیستم
- پشتیبانی از چند کاربر و چند پروتکل، عملیات تجسم صفحه وب
- پروتکل های پشتیبانی شده: vmess، vless، trojan، shadowsocks، dokodemo-door، socks، http
- پشتیبانی برای پیکربندی تنظیمات حمل و نقل بیشتر
- آمار ترافیک، محدودیت ترافیک، محدود کردن زمان انقضا
- قالب های پیکربندی xray قابل تنظیم
- پشتیبانی از پنل دسترسی https (نام دامنه خود ارائه شده + گواهی ssl)
- پشتیبانی از برنامه گواهینامه SSL با یک کلیک و تمدید خودکار
- برای موارد پیکربندی پیشرفته تر، برای جزئیات به پنل مراجعه کنید

# آموزش نصب

#### برای Debian ورژن 8 به بالا 
```
bash <(curl -Ls  https://raw.githubusercontent.com/abdal-security-group/persian-x-ui/main/debianx64-installer.sh)
```

#### برای CentOS ورژن 7 به بالا 
```
bash <(curl -Ls  https://raw.githubusercontent.com/abdal-security-group/persian-x-ui/main/centosx64-installer.sh)
```

#### برای Ubuntu ورژن 16 به بالا 
```
bash <(curl -Ls  https://raw.githubusercontent.com/abdal-security-group/persian-x-ui/main/ubuntux64-installer.sh)
```

## نصب و ارتقاء دستی 
 
> اگر معماری cpu سرور شما "amd64" نیست، "amd64" را در دستور با معماری های دیگر جایگزین کنید.

```
cd /root/
rm x-ui/ /usr/local/x-ui/ /usr/bin/x-ui -rf
tar zxvf x-ui-linux-amd64.tar.gz
chmod +x x-ui/x-ui x-ui/bin/xray-linux-* x-ui/x-ui.sh
cp x-ui/x-ui.sh /usr/bin/x-ui
cp -f x-ui/x-ui.service /etc/systemd/system/
mv x-ui/ /usr/local/
systemctl daemon-reload
systemctl enable x-ui
systemctl restart x-ui
```

 

## استفاده از ربات تلگرام 

- توکن ربات تلگرام
- Tg Bot ChatId
- زمان اجرای چرخه ربات تلگرام با استفاده از نحو crontab

نحو مرجع:
- 30 * * * * * //در 30 دقیقه هر دقیقه اطلاع دهید
- @hourly // اطلاع رسانی ساعتی
- @daily //اعلان هر روز (0:00 صبح)
- @هر 8 ساعت // هر 8 ساعت یکبار اطلاع دهید

محتوای اعلان ربات تلگرام:
- گزارش  ترافیک سرور
- یادآوری ورود به پنل
- یادآوری انقضای گره
- یادآوری هشدار ترافیک

 
##  سیستم عامل های پشتیبان شده

- CentOS 7+
- Ubuntu 16+
- Debian 8+

 
 ⚠️ سلب مسئولیت قانونی ⚠️
 استفاده از x-ui-persian برای حمله به اهداف بدون رضایت قبلی غیرقانونی است. این مسئولیت کاربر نهایی است که از همه قوانین محلی، ایالتی و فدرال قابل اجرا تبعیت کند. اعضای تیم ابدال هیچ مسئولیتی در قبال هرگونه سوء استفاده یا آسیب ناشی از این برنامه ندارند.
 

## ❤️ کمک ها مالی به پروژه 
> https://donate.abdalagency.ir/ 


## گزارش خطا در این پروژه 

 اگر باخطایی مواجه شدید لطفاً به Prof.Shafiei@Gmail.com گرازش کنید تا ما در کمترین زمان آن خطا را رفع کنیم

