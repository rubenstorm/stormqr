
# ⚡ StormQR – Branded Animated QR Codes for Hugo

**StormQR** is a powerful and elegant [Hugo shortcode](https://gohugo.io/content-management/shortcodes/) built by [Ruben Storm](https://github.com/rubenstorm). It generates animated, theme-aware QR codes with crypto icon overlays, clipboard functionality, and branding support — all in a clean, modern UI.

Perfect for sharing Lightning addresses, crypto wallets, email links, or any string of data in a stylish, interactive way.

---

## 🚀 Get Started

### 📦 Manual Installation

1. **Download the shortcode file**  
   Place `stormqr.html` into:  
   `layouts/shortcodes/stormqr.html`

2. **(Optional)** Add your branding logo:  
   Place your SVG logo at:  
   `static/images/stormqr-logo.svg`  
   _(or change the path inside the shortcode)_

3. **Use it in your Hugo content files:**

```go-html-template
{{< stormqr data="https://example.com" >}}
```

---

## ✨ Features

| Feature              | Description                            |
| -------------------- | -------------------------------------- |
| QR code rendering    | Converts any text or URL to QR         |
| Copy to clipboard    | Clickable icon to copy content         |
| Crypto icons         | Trust Wallet CDN or Lightning zap icon |
| Lightning animation  | Pulse effect for zap-enabled QR        |
| Dark mode support    | Theme-aware appearance                 |
| Glassmorphism design | Sleek, modern UI                       |
| Custom branding      | SVG logo or fallback text              |
| Responsive alignment | Align left, center, or right           |
| Toast notification   | Visual feedback when copied            |

---

## 📄 Parameters

### 🔒 Required

| Parameter | Description          | Default  |
| --------- | -------------------- | -------- |
| `data`    | QR content to encode | *(none)* |

---

### 🛠️ Optional

| Parameter    | Description                                                  | Default   |
| ------------ | ------------------------------------------------------------ | --------- |
| `title`      | Tooltip on icon (on hover/tap)                               | `Copy QR` |
| `identifier` | Blockchain or type (`lightning`, `btc`, `eth`, `tron`, etc.) | *none*    |
| `logo`       | Show branding logo (`true` / `false`)                        | `true`    |
| `align`      | Position block: `left`, `center`, `right`                    | `center`  |

---

## 💡 Example Usages

### 🟢 Basic QR Code

```go-html-template
{{< stormqr data="https://example.com" >}}
```

---

### ⚡ Lightning Address (animated icon)

```go-html-template
{{< stormqr data="lnurl1dp68gurn8ghj7mrww4exctnrdakj7tmxx43k2" identifier="lightning" >}}
```

---

### ₿ Bitcoin Wallet

```go-html-template
{{< stormqr data="bc1qxyz..." identifier="bitcoin" >}}
```

---

### 🌐 Ethereum Address

```go-html-template
{{< stormqr data="0xabc123..." identifier="ethereum" >}}
```

---

### 🤖 Arbitrum Wallet

```go-html-template
{{< stormqr data="0xabc123..." identifier="arbitrum" >}}
```

---

### 🕸 Tron Wallet

```go-html-template
{{< stormqr data="TXYZ123abc..." identifier="tron" >}}
```

---

### 🎯 Custom Tooltip

```go-html-template
{{< stormqr data="info@example.com" title="Copy email address" >}}
```

---

### 🎛️ Custom Alignment

```go-html-template
{{< stormqr data="LEFT" align="left" >}}
{{< stormqr data="RIGHT" align="right" >}}
```

These align the QR block to the left and right, respectively.
When not set, the default alignment is `center`.

---

### 🚫 Disable Branding Logo

```go-html-template
{{< stormqr data="123456" logo="false" >}}
```

Shows text: *Powered by Ruben Storm* instead of the logo.

---

### 🔇 Hide Icon (QR only)

```go-html-template
{{< stormqr data="static content" identifier="false" >}}
```

No icon, just the QR image.

---

## 🧱 File Structure

```
stormqr/
├── layouts/
│   └── shortcodes/
│       └── stormqr.html
├── static/
│   └── images/
│       └── stormqr-logo.svg
├── README.md
└── LICENSE.md
```

---

## 📄 License

StormQR is licensed under the [MIT License](./LICENSE.md).
You are free to use it in personal or commercial projects.

---

## 🙌 Contributions & Credits

Built by **Ruben Storm** to add elegant, Lightning-friendly QR codes to his nomadic websites.

Inspired by minimalist design, Web3 aesthetics, and a love for open-source.

* GitHub: [github.com/rubenstorm/stormqr](https://github.com/rubenstorm/stormqr)
* Forks and pull requests are welcome ❤️

---

## 💖 Support

If StormQR is useful to you, zap me some sats ⚡
Every ⚡ helps fund more open-source experiments.

👉 **[coinos.io/rubenstorm](https://coinos.io/rubenstorm)**

Danke schön 🙏


