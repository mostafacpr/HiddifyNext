


## بر اساس سیستم عامل خود یکی از موارد زیر را انتخاب نمایید.
 
 ## ن ب روی آندروید (کلیک کنید)  

### با فیلترشکن خاموش روی لینک دریافتی کلیک میکنیم درصفحه بازشده روی قسمت قرمز رنگ ( کلیک برای اعمال فیلترشکن) میزنیم .
<div dir=”rtl”>
اگر برنامه هیدیفای نکست روندارید از صفحه ظاهر شده دکمه دانلود رو بزنید ونصب کنید پس از نصب دوباره دکمه قرمز رنگ ( کلیک برای اعمال یلترشکن) میزنیم وسپس دکمه سبز رنگ بارگذاری در برنامه رو میزنیم تا در برنامه هیدیفای نکست بارگذاری شود
و سپس دکمه اتصال رو میزنیم .

فیلم آموزشی
 
 نصب روی آیفون
برنامه Streisand  (دانلود از استور)

با فیلترشکن خاموش روی لینک دریافتی کلیک میکنیم

درصفحه بازشده روی قسمت قرمز رنگ ( کلیک برای اعمال فیلترشکن) میزنیم .

و فلش نرم افزار های بیشتر رو میزنیم .


و دکمه سبز رنگ بارگذاری در برنامه کنار برنامه streisand رو میزنم تا کانفیگ ها در برنامه وارد بشه سپس دکمه connect رو میزنیم.

فیلم آموزشی

گزینه Setting > subscription > update on open رو هم بزنین . تا در هربار بازشدن برنامه کانفیگ های جدید رو دریافت کنه. طبق فیلم پایین


فیلم آموزشی
 
 نصب روی ویندوز (کلیک کنید) نسخه portable
 
 نصب روی مک (کلیک کنید)

نصب روی لینوکس (کلیک کنید)

![alt text](https://frp.free.nf/wp-content/uploads/2023/11/ios.mp4 "Title")

🎥 ویدئوی مرتبط با هیدیفای‌نکست
</div>


<details>
<summary>برنامه هیدیفای</summary>
<br>
 
نصب روی ویندوز (کلیک کنید) نسخه portable
 
 نصب روی مک (کلیک کنید)

نصب روی لینوکس (کلیک کنید)
</details>


اصول مهندسی نرم افزار ، از کتاب Robert Code Martin [*Clean Code*](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882) ، اقتباس گرفته شده است تا در این نوشته اصول آن برای زبان برنامه نویسی PHP را بررسی کنیم. این یک راهنمای ساده نیست. این یک راهنما برای تولید نرم افزارهای قابل خواندن با خوانایی بالا، قابل استفاده مجدد در زبان برنامه نویسی پی اچ پی است.

__salam ali__
*salam ali*

(https://m.fix7.shop)[non]

[camelCase](https://camelcase.ir/)🌳🍉🍉🌷 📷  ☕

---

<div dir=”rtl”>

متن خود را بنویسید….


{
  "log": {
    "access": "",
    "error": "",
    "loglevel": "warning"
  },
  "inbounds": [
    {
      "tag": "socks",
      "port": 10808,
      "listen": "127.0.0.1",
      "protocol": "socks",
      "sniffing": {
        "enabled": true,
        "destOverride": [
          "http",
          "tls"
        ],
        "routeOnly": false
      },
      "settings": {
        "auth": "noauth",
        "udp": true,
        "allowTransparent": false
      }
    },
    {
      "tag": "http",
      "port": 10809,
      "listen": "127.0.0.1",
      "protocol": "http",
      "sniffing": {
        "enabled": true,
        "destOverride": [
          "http",
          "tls"
        ],
        "routeOnly": false
      },
      "settings": {
        "auth": "noauth",
        "udp": true,
        "allowTransparent": false
      }
    }
  ],
  "outbounds": [
    {
      "tag": "proxy",
      "protocol": "vless",
      "settings": {
        "vnext": [
          {
            "address": "###CLEANIP###",
            "port": "443",
            "users": [
              {
                "id": "###UUID###",
                "alterId": 0,
                "email": "t@t.tt",
                "security": "auto",
                "encryption": "none",
                "flow": ""
              }
            ]
          }
        ]
      },
      "streamSettings": {
        "network": "ws",
        "security": "tls",
        "tlsSettings": {
          "allowInsecure": true,
          "serverName": "p2.IPcL.tOP",
          "alpn": [
            "h2",
            "http/1.1"
          ],
          "fingerprint": "chrome",
          "show": false
        },
        "wsSettings": {
          "path": "/NcnELaMKKFprtS7GqudEw78d/?ed=2048",
          "headers": {
            "Host": "p2.IPcL.tOP"
          }
        },
        "sockopt": {
          "dialerProxy": "fragment",
          "tcpKeepAliveIdle": 100,
          "mark": 255
        }
      },
      "mux": {
        "enabled": false,
        "concurrency": -1
      }
    },
    {
      "tag": "fragment",
      "protocol": "freedom",
      "settings": {
        "fragment": {
          "packets": "tlshello",
          "length": "10-20",
          "interval": "10-20"
        }
      },
      "streamSettings": {
        "sockopt": {
          "TcpNoDelay": true,
          "tcpKeepAliveIdle": 100,
          "mark": 255
        }
      }
    },
    {
      "tag": "direct",
      "protocol": "freedom",
      "settings": {}
    },
    {
      "tag": "block",
      "protocol": "blackhole",
      "settings": {
        "response": {
          "type": "http"
        }
      }
    }
  ],
  "routing": {
    "domainStrategy": "AsIs",
    "rules": [
      {
        "type": "field",
        "inboundTag": [
          "api"
        ],
        "outboundTag": "api",
        "enabled": true
      },
      {
        "id": "5465425548310166497",
        "type": "field",
        "outboundTag": "direct",
        "domain": [
          "domain:ir",
          "geosite:cn"
        ],
        "enabled": true
      },
      {
        "id": "5425034033205580637",
        "type": "field",
        "outboundTag": "direct",
        "ip": [
          "geoip:private",
          "geoip:cn",
          "geoip:ir"
        ],
        "enabled": true
      },
      {
        "id": "5627785659655799759",
        "type": "field",
        "port": "0-65535",
        "outboundTag": "proxy",
        "enabled": true
      }
    ]
  }
}
