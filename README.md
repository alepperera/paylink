# PayLink

PayLink is a payment organizer and an open source alternative to [Paynest](https://paynest.app).

## Live example

[https://paylink-danielcastillo.netlify.app/](https://paylink-danielcastillo.netlify.app/)

## How to use

PayLink uses React and Boostrap to create pre-built components for your PayLink page. You only need to work in the **paylink.config.json** file.

### Theme

You can modify the theme in the **theme** property. It accepts 4 values: minimalist-theme, minimalist-dark-theme, swordfest-theme and swordfest-dark-theme.

### Hero section

The Hero section is going to have your photo, name and description. You can modify it in the **properties** object which has the following properties.

- name: your name
- description: your description
- alt: an alternative text for your photo
- hero: the path to your photo. We recommend to put it in the **images** folder.

For example:

    "properties": {
        "name": "Daniel Castillo",
        "description": "Frontend web developer",
        "alt": "Photo of Daniel Castillo",
        "hero": "./src/images/daniel-castillo.png"
    },

### Social media section

The Social Media section is going to have all your social media links. You can modify it in the **Social** array which has one object per social media. You only need to put your social media link in the **link** property within the corresponding object.

For example:

    "Social": [
        { "label": "Link", "type": "link", "link": "https://danielcastillop.netlify.app" },
        { "label": "GitHub", "type": "github", "link": "https://github.com/dlcastillop" },
        { "label": "Twitter", "type": "twitter", "link": "https://twitter.com/dlcastillop" },
        { "label": "LinkedIn", "type": "linkedin", "link": "https://linkedin.com/in/dlcastillop" },
        { "label": "Instagram", "type": "instagram", "link": "https://instagram.com/dlcastillop" },
        { "label": "Discord", "type": "discord", "link": "" },
        { "label": "Facebook", "type": "facebook", "link": "" },
        { "label": "Medium", "type": "medium", "link": "" },
        { "label": "Pinterest", "type": "pinterest", "link": "" },
        { "label": "Snapchat", "type": "snapchat", "link": "" },
        { "label": "Telegram", "type": "telegram", "link": "" },
        { "label": "TikTok", "type": "tiktok", "link": "" },
        { "label": "Twitch", "type": "twitch", "link": "" },
        { "label": "Vimeo", "type": "vimeo", "link": "" },
        { "label": "WhatsApp", "type": "whatsapp", "link": "" },
        { "label": "YouTube", "type": "youtube", "link": "" },
        { "label": "Product Hunt", "type": "product-hunt", "link": "" }
    ],

If you want to modify the order of the social media, you must organize the objects according to your preference.

For example:

    "Social": [
        { "label": "Twitter", "type": "twitter", "link": "https://twitter.com/dlcastillop" },
        { "label": "GitHub", "type": "github", "link": "https://github.com/dlcastillop" },
        { "label": "LinkedIn", "type": "linkedin", "link": "https://linkedin.com/in/dlcastillop" },
        { "label": "Instagram", "type": "instagram", "link": "https://instagram.com/dlcastillop" },
        { "label": "Link", "type": "link", "link": "https://danielcastillop.netlify.app" },
        { "label": "Discord", "type": "discord", "link": "" },
        { "label": "Facebook", "type": "facebook", "link": "" },
        { "label": "Medium", "type": "medium", "link": "" },
        { "label": "Pinterest", "type": "pinterest", "link": "" },
        { "label": "Snapchat", "type": "snapchat", "link": "" },
        { "label": "Telegram", "type": "telegram", "link": "" },
        { "label": "TikTok", "type": "tiktok", "link": "" },
        { "label": "Twitch", "type": "twitch", "link": "" },
        { "label": "Vimeo", "type": "vimeo", "link": "" },
        { "label": "WhatsApp", "type": "whatsapp", "link": "" },
        { "label": "YouTube", "type": "youtube", "link": "" },
        { "label": "Product Hunt", "type": "product-hunt", "link": "" }
    ],

The Social Media section supports Twitter, GitHub, LinkedIn, Instagram, a link, Discord, Facebook, Medium, Pinterest, Snapchat, Telegram, TikTok, Twitch, Vimeo, WhatsApp, YouTube and Product Hunt.

### Payment section

The Payment section is going to have all your payment methods. You can modify it in the **Payments** array which has one object per payment methods. You only need to put your payment method link in the **value** property within the corresponding object.

For example:

    "Payments": [
        {
            "id": "btc",
            "label": "Bitcoin",
            "value": "bc1qejahgjmqnmyrw7jvn0d7evfdq6ssjl3wq7hfle",
            "img": "./src/images/crypto/btc.svg"
        },
        {
            "id": "busd",
            "label": "BinanceUSD",
            "value": "",
            "img": "./src/images/crypto/busd.svg"
        },
        {
            "id": "matic",
            "label": "Matic",
            "value": "",
            "img": "./src/images/crypto/matic.svg"
        },
        {
            "id": "doge",
            "label": "DogeCoin",
            "value": "",
            "img": "./src/images/crypto/doge.svg"
        },
        {
            "id": "eth",
            "label": "Ethereum",
            "value": "0x59C864f658caD68A19a97499755080c056079988",
            "img": "./src/images/crypto/eth.svg"
        },
        {
            "id": "ltc",
            "label": "Litecoin",
            "value": "",
            "img": "./src/images/crypto/ltc.svg"
        },
        {
            "id": "paypal",
            "label": "Paypal",
            "value": "",
            "img": "./src/images/crypto/paypal.svg"
        },
        {
            "id": "usdt",
            "label": "USDT",
            "value": "",
            "img": "./src/images/crypto/usdt.svg"
        },
        {
            "id": "qvapay",
            "label": "QvaPay",
            "value": "https://qvapay.com/payme/dlcastillop",
            "img": "./src/images/crypto/qvapay.svg"
        },
        {
            "id": "sol",
            "label": "Solana",
            "value": "",
            "img": "./src/images/crypto/sol.svg"
        },
        {
            "id": "ada",
            "label": "ADA",
            "value": "",
            "img": "./src/images/crypto/ada.svg"
        },
        {
            "id": "trx",
            "label": "Tron",
            "value": "",
            "img": "./src/images/crypto/trx.svg"
        },
        {
            "id": "xrp",
            "label": "XRP",
            "value": "",
            "img": "./src/images/crypto/xrp.svg"
        },
        {
            "id": "card",
            "label": "Card",
            "value": "",
            "img": "./images/payments/card.svg"
        }
    ]

If you want to modify the order of the payment methods, you must organize the objects according to your preference.

For example:

    "Payments": [
        {
            "id": "qvapay",
            "label": "QvaPay",
            "value": "https://qvapay.com/payme/dlcastillop",
            "img": "./src/images/crypto/qvapay.svg"
        },
        {
            "id": "eth",
            "label": "Ethereum",
            "value": "0x59C864f658caD68A19a97499755080c056079988",
            "img": "./src/images/crypto/eth.svg"
        },
        {
            "id": "btc",
            "label": "Bitcoin",
            "value": "bc1qejahgjmqnmyrw7jvn0d7evfdq6ssjl3wq7hfle",
            "img": "./src/images/crypto/btc.svg"
        },
        {
            "id": "busd",
            "label": "BinanceUSD",
            "value": "",
            "img": "./src/images/crypto/busd.svg"
        },
        {
            "id": "matic",
            "label": "Matic",
            "value": "",
            "img": "./src/images/crypto/matic.svg"
        },
        {
            "id": "doge",
            "label": "DogeCoin",
            "value": "",
            "img": "./src/images/crypto/doge.svg"
        },
        {
            "id": "ltc",
            "label": "Litecoin",
            "value": "",
            "img": "./src/images/crypto/ltc.svg"
        },
        {
            "id": "paypal",
            "label": "Paypal",
            "value": "",
            "img": "./src/images/crypto/paypal.svg"
        },
        {
            "id": "usdt",
            "label": "USDT",
            "value": "",
            "img": "./src/images/crypto/usdt.svg"
        },
        {
            "id": "sol",
            "label": "Solana",
            "value": "",
            "img": "./src/images/crypto/sol.svg"
        },
        {
            "id": "ada",
            "label": "ADA",
            "value": "",
            "img": "./src/images/crypto/ada.svg"
        },
        {
            "id": "trx",
            "label": "Tron",
            "value": "",
            "img": "./src/images/crypto/trx.svg"
        },
        {
            "id": "xrp",
            "label": "XRP",
            "value": "",
            "img": "./src/images/crypto/xrp.svg"
        },
        {
            "id": "card",
            "label": "Card",
            "value": "",
            "img": "./images/payments/card.svg"
        }
    ]

The Payment section supports Bitcoin, Binance USD, Matic, DogeCoin, Ethereum, Litecoin, PayPal, USDT, QvaPay, Solana, ADA, TRON, XRP and a card.

## Special thanks

Many thanks to [Manuel Ernesto](https://twitter.com/manuelernestog), [Yoannis Sánchez](https://twitter.com/yossthedev), [Carlos Z. Bent](https://t.me/carloszbent_channel) and [Alex Navarro](https://twitter.com/Swordfest). PayLink is much better thanks to your work.

## Contributions

Suggestions and pull requests are welcomed!
