# rules

Personal rules, maintained by Muse for Wen Ze. Synced daily from upstream, so the lists stay fresh without hand-editing.

## Services

| Service | Surge | Loon | Shadowrocket |
|---|---|---|---|
| AI | `rule/Surge/AI.list` | `rule/Loon/AI.list` | `rule/Shadowrocket/AI.list` |
| Telegram | `rule/Surge/Telegram.list` | `rule/Loon/Telegram.list` | `rule/Shadowrocket/Telegram.list` |
| WhatsApp | `rule/Surge/Whatsapp.list` | `rule/Loon/Whatsapp.list` | `rule/Shadowrocket/Whatsapp.list` |
| Instagram | `rule/Surge/Instagram.list` | `rule/Loon/Instagram.list` | `rule/Shadowrocket/Instagram.list` |
| TikTok | `rule/Surge/TikTok.list` | `rule/Loon/TikTok.list` | `rule/Shadowrocket/TikTok.list` |
| YouTube | `rule/Surge/YouTube.list` | `rule/Loon/YouTube.list` | `rule/Shadowrocket/YouTube.list` |
| Netflix | `rule/Surge/Netflix.list` | `rule/Loon/Netflix.list` | `rule/Shadowrocket/Netflix.list` |

## Sources

- Telegram, WhatsApp, Instagram, TikTok, YouTube, Netflix: [blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script) (mirrored as-is).
- AI: [Sukka's ai.conf](https://ruleset.skk.moe/List/non_ip/ai.conf) plus curated extras in `scripts/ai-extra.list`. Only AI services. No broad shared domains (no bing.com, googleapis.com, gstatic.com, auth0.com, stripe.com, sentry.io). Those would hijack unrelated traffic.

Surge, Loon and Shadowrocket use almost the same format, so the three files carry the same domains. The only difference: Surge keeps the Gemini `URL-REGEX` redirect rule, Loon / Shadowrocket drop it (not reliable in their remote lists). Gemini itself is still covered.

## Use

Replace the policy name with your own policy group name.

### Surge, in `[Rule]`

```
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Telegram.list,香港
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Whatsapp.list,香港
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Instagram.list,香港
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/TikTok.list,日本
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/YouTube.list,香港
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/Netflix.list,香港
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Surge/AI.list,美国
```

### Loon, add as Remote Rule

```
https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Telegram.list
https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Whatsapp.list
https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Instagram.list
https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/TikTok.list
https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/YouTube.list
https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/Netflix.list
https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Loon/AI.list
```

### Shadowrocket, in `[Rule]`

```
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Telegram.list,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Whatsapp.list,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Instagram.list,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/TikTok.list,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/YouTube.list,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/Netflix.list,PROXY
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/rules@main/rule/Shadowrocket/AI.list,PROXY
```

## Daily sync

`.github/workflows/sync-rules.yml` runs every day at 09:00 Asia/Shanghai (01:00 UTC). It pulls the latest lists from blackmatrix7 and Sukka, rebuilds the AI lists (Sukka + `scripts/ai-extra.list`), and commits + pushes only when something changed. No hand-editing needed.

To add your own domain or a new service, edit the list (or `scripts/ai-extra.list` for AI) and push; the next sync keeps your edit unless upstream also changed that file. To force a sync now, run the workflow manually from the repo's Actions tab.

## Update

Edit the list, push, refresh the rule in the app. No need to re-add the link.
