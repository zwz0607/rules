# rules

Personal rules, maintained by Muse for Wen Ze. Synced daily from upstream, so the lists stay fresh without hand-editing.

## Services

| Service | Surge | Loon | Shadowrocket |
|---|---|---|---|
| Telegram | `rule/Surge/Telegram.list` | `rule/Loon/Telegram.list` | `rule/Shadowrocket/Telegram.list` |
| Whatsapp | `rule/Surge/Whatsapp.list` | `rule/Loon/Whatsapp.list` | `rule/Shadowrocket/Whatsapp.list` |
| Instagram | `rule/Surge/Instagram.list` | `rule/Loon/Instagram.list` | `rule/Shadowrocket/Instagram.list` |
| TikTok | `rule/Surge/TikTok.list` | `rule/Loon/TikTok.list` | `rule/Shadowrocket/TikTok.list` |
| YouTube | `rule/Surge/YouTube.list` | `rule/Loon/YouTube.list` | `rule/Shadowrocket/YouTube.list` |
| Netflix | `rule/Surge/Netflix.list` | `rule/Loon/Netflix.list` | `rule/Shadowrocket/Netflix.list` |
| AI | `rule/Surge/AI.list` | `rule/Loon/AI.list` | `rule/Shadowrocket/AI.list` |

## Sources

- Telegram, WhatsApp, Instagram, TikTok, YouTube, Netflix: [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script) (mirrored as-is).
- AI: [Sukka's ai.conf](https://ruleset.skk.moe/List/non_ip/ai.conf) plus curated extras in `scripts/ai-extra.list`. Only AI services. No broad shared domains (no bing.com, googleapis.com, gstatic.com, auth0.com, stripe.com, sentry.io). Those would hijack unrelated traffic.

Surge, Loon and Shadowrocket use almost the same format, so the three files carry the same domains. The only difference: Surge keeps the Gemini `URL-REGEX` redirect rule, Loon / Shadowrocket drop it (not reliable in their remote lists). Gemini itself is still covered.

## Use

直接复制下面链接，粘贴进 App 的规则集订阅就行，不用写 RULE-SET。更新间隔 86400。

### Surge

#### Telegram

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Telegram.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Telegram.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Telegram.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Telegram.list)

#### Whatsapp

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Whatsapp.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Whatsapp.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Whatsapp.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Whatsapp.list)

#### Instagram

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Instagram.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Instagram.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Instagram.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Instagram.list)

#### TikTok

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/TikTok.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/TikTok.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/TikTok.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/TikTok.list)

#### YouTube

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/YouTube.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/YouTube.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/YouTube.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/YouTube.list)

#### Netflix

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Netflix.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Netflix.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Netflix.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/Netflix.list)

#### AI

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/AI.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/AI.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/AI.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Surge/AI.list)

### Loon

#### Telegram

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Telegram.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Telegram.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Telegram.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Telegram.list)

#### Whatsapp

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Whatsapp.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Whatsapp.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Whatsapp.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Whatsapp.list)

#### Instagram

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Instagram.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Instagram.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Instagram.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Instagram.list)

#### TikTok

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/TikTok.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/TikTok.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/TikTok.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/TikTok.list)

#### YouTube

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/YouTube.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/YouTube.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/YouTube.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/YouTube.list)

#### Netflix

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Netflix.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Netflix.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Netflix.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/Netflix.list)

#### AI

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/AI.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/AI.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/AI.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Loon/AI.list)

### Shadowrocket

#### Telegram

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Telegram.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Telegram.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Telegram.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Telegram.list)

#### Whatsapp

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Whatsapp.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Whatsapp.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Whatsapp.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Whatsapp.list)

#### Instagram

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Instagram.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Instagram.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Instagram.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Instagram.list)

#### TikTok

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/TikTok.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/TikTok.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/TikTok.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/TikTok.list)

#### YouTube

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/YouTube.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/YouTube.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/YouTube.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/YouTube.list)

#### Netflix

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Netflix.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Netflix.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Netflix.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/Netflix.list)

#### AI

CDN（推荐）: [https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/AI.list](https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/AI.list)

Raw: [https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/AI.list](https://raw.githubusercontent.com/zwz0607/rules/main/rule/Shadowrocket/AI.list)

## Daily sync

`.github/workflows/sync-rules.yml` runs every day at 09:00 Asia/Shanghai (01:00 UTC). It pulls the latest lists from blackmatrix7 and Sukka, rebuilds the AI lists (Sukka + `scripts/ai-extra.list`), and commits + pushes only when something changed. No hand-editing needed.

To add your own domain or a new service, edit the list (or `scripts/ai-extra.list` for AI) and push; the next sync keeps your edit unless upstream also changed that file. To force a sync now, run the workflow manually from the repo's Actions tab.

## Update

Edit the list, push, refresh the rule in the app. No need to re-add the link.
