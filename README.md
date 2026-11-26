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

订阅链接在各 App 文件夹下的服务文件夹里，例如 [rule/Surge/Whatsapp](rule/Surge/Whatsapp)：点进服务文件夹，看 README 复制链接。

## Daily sync

`.github/workflows/sync-rules.yml` runs every day at 09:00 Asia/Shanghai (01:00 UTC). It pulls the latest lists from blackmatrix7 and Sukka, rebuilds the AI lists (Sukka + `scripts/ai-extra.list`), and commits + pushes only when something changed. No hand-editing needed.

To add your own domain or a new service, edit the list (or `scripts/ai-extra.list` for AI) and push; the next sync keeps your edit unless upstream also changed that file. To force a sync now, run the workflow manually from the repo's Actions tab.

## Update

Edit the list, push, refresh the rule in the app. No need to re-add the link.
