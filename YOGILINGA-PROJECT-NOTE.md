# 🪷 Dự Án Yogi & Linga — Project Brain

> **Khi muốn tiếp tục:** Chỉ cần nhắn *"tiếp tục làm dự án yogilinga"* — đọc note này là đủ để biết đang ở đâu và làm gì tiếp theo.

---

## 📌 Tổng Quan

| Mục | Thông tin |
|---|---|
| **Tên site** | Yogi & Linga |
| **Mô tả** | Blog sexual wellness — review sản phẩm, hướng dẫn mua, bài viết sức khỏe |
| **URL live** | https://sontis98.github.io/yogilinga/ |
| **GitHub repo** | https://github.com/Sontis98/yogilinga |
| **GitHub user** | Sontis98 |
| **Tech stack** | Jekyll (github-pages gem) + GitHub Actions |
| **Local folder** | `D:\project\yogilinga` |

---

## 🔑 Credentials & Config Quan Trọng

```
GitHub PAT: [xem trong Obsidian — không lưu trên GitHub vì bị push protection]
Tạo tại: GitHub → Settings → Developer settings → Personal access tokens → Classic
Permissions cần: repo + workflow
```

### _config.yml (các setting quan trọng)
```yaml
baseurl: "/yogilinga"   # ← KHÔNG được xoá, site host trên subdirectory
url: "https://sontis98.github.io"
include: ["_pages"]     # ← BẮT BUỘC — Jekyll mới process _pages/
```

> Khi chuyển sang domain riêng `yogilinga.com`: đổi `baseurl: ""` và `url: "https://yogilinga.com"`

---

## ⚠️ Quy Trình Push Code (BẮT BUỘC)

**KHÔNG push trực tiếp từ `D:\project\yogilinga`** — Windows mount làm hỏng `.git/config`.

**KHÔNG dùng Write/Edit tools cho layout files** — tạo null bytes → Jekyll đọc binary → build fail.

**Luôn làm theo flow này:**

```bash
# 1. Clone mới vào /tmp (mỗi session) — dùng PAT từ Obsidian
git clone https://PAT_HERE@github.com/Sontis98/yogilinga.git /tmp/yogi_session

# 2. Viết file qua Python nếu content có backtick, hoặc bash cat nếu không
python3 -c "open('/tmp/yogi_session/path/file','w').write(content)"

# 3. Kiểm tra null bytes trước khi push
python3 -c "c = open('/tmp/yogi_session/_layouts/default.html','rb').read(); print(c.count(b'\\x00'))"

# 4. Commit và push
cd /tmp/yogi_session && git add . && git config user.email "ssontiss@gmail.com" && git config user.name "Sontis98" && git commit -m "feat: ..." && git push origin main
```

> Bash mount path: `/sessions/sleepy-relaxed-wright/mnt/yogilinga/`
> Gemfile.lock bị `.gitignore` (Windows platform không tương thích Linux CI)
> **Dùng Python để write file nếu content có backtick** — heredoc sẽ bị break

---

## 🏗️ Cấu Trúc Site Hiện Tại

```
D:\project\yogilinga\
├── _config.yml              # include: [_pages] — QUAN TRỌNG
├── _layouts/
│   ├── default.html         # GA4, Schema JSON-LD, age gate, nav, footer
│   ├── review.html          # Schema Review JSON-LD, scorecard, buy box, related guide, more from brand
│   ├── post.html            # Layout wellness posts
│   └── guide.html           # Layout guides + related reviews + more guides
├── _reviews/                # 40 reviews (với related_guide_url front matter)
├── _posts/                  # 8 wellness blog posts
├── _guides/                 # 7 buying guides (với related_brand/related_brands front matter)
├── _pages/
│   ├── reviews.html         # /reviews/ — filter JS hoạt động ✅
│   ├── wellness.html        # /wellness/
│   ├── guides.html          # /guides/
│   ├── about.md             # Scoring rubric, 3 team personas, affiliate transparency ✅
│   ├── contact.md           # Form mailto hoạt động ✅
│   ├── affiliate-disclosure.md  # Đúng programs (Lovense, We-Vibe, LELO...) ✅
│   ├── privacy.md           # GA4 G-071MTW1DP2, GDPR/CCPA ✅
│   └── terms.md             # Comprehensive ✅
├── assets/
│   ├── css/main.css
│   └── images/
│       ├── reviews/         # 40 JPEGs on-brand
│       ├── blog/            # 17 JPEGs lifestyle
│       └── guides/          # 7 JPEGs
├── index.html               # Homepage
├── robots.txt
└── google3749be6f9e4e8e72.html
```

---

## ✅ Đã Làm Xong

- [x] **40 reviews** — Lovense (10), We-Vibe (5), Satisfyer (5), Womanizer (5), Dame (5), LELO (5), b-Vibe (5)
- [x] **7 buying guides** — body-safe materials, first vibrator, app toys, lubricant, anal toys, couples toys, LELO brand
- [x] **8 wellness blog posts**
- [x] **64 ảnh** tự generate (on-brand, gradient theo màu từng brand, score badge)
- [x] **Filter buttons /reviews/** — hoạt động đúng (All / Vibrators / App-Controlled / Couples / Luxury / Anal)
- [x] **Contact form** — gửi mailto thật
- [x] **SEO:** GA4 `G-071MTW1DP2`, Search Console verified, sitemap submitted
- [x] **Schema JSON-LD** Review markup
- [x] **GitHub Actions** updated configure-pages@v5
- [x] **Internal linking** — 30 reviews có related_guide_url, 7 guides có related_brand
- [x] **Legal pages** — Affiliate Disclosure (đúng programs), Privacy (GA4 confirmed), Terms (comprehensive)
- [x] **About page** — Scoring rubric 6 criteria, 3 team personas, affiliate transparency section

---

## 📋 VIỆC CẦN LÀM TIẾP — Theo Thứ Tự Ưu Tiên

### 🔴 Trước khi đăng ký Affiliate (USER action)

1. **Mua domain `yogilinga.com`** (~$10–15/năm tại Namecheap)
   - Sau khi mua: đổi `_config.yml` → `baseurl: ""`, `url: "https://yogilinga.com"`
   - Cài custom domain trong GitHub Pages settings
   - GitHub sẽ tự cấp SSL cert (Let's Encrypt)
   - `.github.io` subdomain bị một số affiliate programs reject tự động

### 🟡 Đăng Ký Affiliate Programs (sau khi có domain)

| Brand | Network | Commission | Cookie |
|---|---|---|---|
| Lovense | Direct program | ~15–20% | 30 ngày |
| We-Vibe | Impact Radius | ~10–15% | 30 ngày |
| LELO | ShareASale | ~10% | 45 ngày |
| Womanizer | ShareASale | ~10–12% | 30 ngày |
| Dame | Impact Radius / direct | ~10% | 30 ngày |
| Satisfyer | ShareASale | ~10% | 30 ngày |
| b-Vibe | ShareASale | ~10% | 30 ngày |

> Sau khi có affiliate link thật: thay placeholder `buy_url` trong tất cả 40 `_reviews/*.md`

### 🟢 Nội Dung & SEO (có thể làm ngay)

- [ ] **Thêm reviews mới**: Aneros, Hot Octopuss, Njoy
- [ ] **5–10 bài wellness posts mới**
- [ ] **Meta description** optimize từng trang
- [ ] **Newsletter signup** — email capture (ConvertKit hoặc Mailchimp free tier)
- [ ] **Internal linking** — wellness posts → reviews liên quan

---

## 🎨 Design System

| Token | Giá trị |
|---|---|
| Font serif | Cormorant Garamond |
| Font sans | Jost |
| Background | `#1a0f0f` (dark wine) |
| Accent | `--rose-gold` (#C9956C) |
| Text | `--cream` (#F5E6D7), `--cream-dim` (#B4A091) |

**Breakpoints:** 900px (2-col → 3-col), 600px (1-col)

---

## 📝 Commit History Quan Trọng

| Commit | Nội dung |
|---|---|
| `dc029c8` | feat: update legal pages + about page for affiliate readiness |
| `48e8434` | feat: internal linking guides ↔ reviews |
| `53ee3f9` | fix: filter buttons + contact form mailto |
| `34efaf0` | feat: 64 ảnh cho toàn bộ site |
| `c5cd9f7` | feat: 10 reviews LELO + b-Vibe |
| `9de20e0` | fix: include _pages → /reviews/ load được |
| `df7d9c9` | fix: null bytes default.html (root cause 404) |

---

## 💡 Ghi Chú Kỹ Thuật

- **NULL BYTE BUG:** Write/Edit tools qua Windows mount → null bytes → Jekyll fail. Dùng `bash cat >` hoặc `python3` để write.
- **HEREDOC + BACKTICK:** Nếu content có backtick (```), dùng Python để write file thay vì heredoc.
- **`include: [_pages]`** trong `_config.yml` là BẮT BUỘC
- **Filter JS** trong reviews.html dùng `data-filters` attribute
- **Images** generate bằng Python Pillow — gradient + score badge — 65KB/file
- **Affiliate programs:** Lovense (direct), We-Vibe + Dame (Impact Radius), LELO + Womanizer + Satisfyer + b-Vibe (ShareASale)

---

*Tạo: 2026-05-24 | Cập nhật: 2026-05-25*
