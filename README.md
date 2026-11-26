# rules

Personal rules, maintained by Muse for Wen Ze. Synced daily from upstream, so the lists stay fresh without hand-editing.

## Services

| Service | Surge | Loon | Shadowrocket |
|---|---|---|---|
| Telegram | `rule/Surge/Telegram/Telegram.list` | `rule/Loon/Telegram/Telegram.list` | `rule/Shadowrocket/Telegram/Telegram.list` |
| Whatsapp | `rule/Surge/Whatsapp/Whatsapp.list` | `rule/Loon/Whatsapp/Whatsapp.list` | `rule/Shadowrocket/Whatsapp/Whatsapp.list` |
| Instagram | `rule/Surge/Instagram/Instagram.list` | `rule/Loon/Instagram/Instagram.list` | `rule/Shadowrocket/Instagram/Instagram.list` |
| TikTok | `rule/Surge/TikTok/TikTok.list` | `rule/Loon/TikTok/TikTok.list` | `rule/Shadowrocket/TikTok/TikTok.list` |
| YouTube | `rule/Surge/YouTube/YouTube.list` | `rule/Loon/YouTube/YouTube.list` | `rule/Shadowrocket/YouTube/YouTube.list` |
| Netflix | `rule/Surge/Netflix/Netflix.list` | `rule/Loon/Netflix/Netflix.list` | `rule/Shadowrocket/Netflix/Netflix.list` |
| AI | `rule/Surge/AI/AI.list` | `rule/Loon/AI/AI.list` | `rule/Shadowrocket/AI/AI.list` |
| Bybit | `rule/Surge/Bybit/Bybit.list` | `rule/Loon/Bybit/Bybit.list` | `rule/Shadowrocket/Bybit/Bybit.list` |
| Google | `rule/Surge/Google/Google.list` | `rule/Loon/Google/Google.list` | `rule/Shadowrocket/Google/Google.list` |
| Facebook | `rule/Surge/Facebook/Facebook.list` | `rule/Loon/Facebook/Facebook.list` | `rule/Shadowrocket/Facebook/Facebook.list` |
| Twitter | `rule/Surge/Twitter/Twitter.list` | `rule/Loon/Twitter/Twitter.list` | `rule/Shadowrocket/Twitter/Twitter.list` |
| GitHub | `rule/Surge/GitHub/GitHub.list` | `rule/Loon/GitHub/GitHub.list` | `rule/Shadowrocket/GitHub/GitHub.list` |
| Spotify | `rule/Surge/Spotify/Spotify.list` | `rule/Loon/Spotify/Spotify.list` | `rule/Shadowrocket/Spotify/Spotify.list` |
| AppStore | `rule/Surge/AppStore/AppStore.list` | `rule/Loon/AppStore/AppStore.list` | `rule/Shadowrocket/AppStore/AppStore.list` |

## Sources

- Telegram, WhatsApp, Instagram, TikTok, YouTube, Netflix, Google, Facebook, Twitter, GitHub, Spotify: [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script) (mirrored as-is).
- AppStore: [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script) (upstream, 2 domains) plus curated extras in `scripts/appstore-extra.list` (download/CDN domains: mzstatic.com, iosapps/osxapps.itunes.apple.com, cdn-apple.com, etc.).
- AI: [Sukka's ai.conf](https://ruleset.skk.moe/List/non_ip/ai.conf) plus curated extras in `scripts/ai-extra.list`. Only AI services. No broad shared domains (no bing.com, googleapis.com, gstatic.com, auth0.com, stripe.com, sentry.io). Those would hijack unrelated traffic.
- Bybit: [v2fly/domain-list-community](https://github.com/v2fly/domain-list-community) (`data/bybit`), synced daily, plus curated extras in `scripts/bybit-extra.list` (RuleGo). blackmatrix7 has no Bybit list.

Surge, Loon and Shadowrocket use almost the same format, so the three files carry the same domains. The only difference: Surge keeps the Gemini `URL-REGEX` redirect rule, Loon / Shadowrocket drop it (not reliable in their remote lists). Gemini itself is still covered.

## Use

订阅链接在各 App 文件夹下的服务文件夹里，例如 [rule/Surge/Whatsapp](rule/Surge/Whatsapp)：点进服务文件夹，看 README 复制链接。

## Daily sync

`.github/workflows/sync-rules.yml` runs every day at 09:00 Asia/Shanghai (01:00 UTC). It pulls the latest lists from blackmatrix7 and Sukka, rebuilds the AI lists (Sukka + `scripts/ai-extra.list`) and the AppStore lists (blackmatrix7 + `scripts/appstore-extra.list`), and commits + pushes only when something changed. No hand-editing needed.

To add your own domain or a new service, edit the list (or `scripts/ai-extra.list` for AI) and push; the next sync keeps your edit unless upstream also changed that file. To force a sync now, run the workflow manually from the repo's Actions tab.

## Update

Edit the list, push, refresh the rule in the app. No need to re-add the link.
