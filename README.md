# surge-rules

Personal AI rules, maintained by Muse for Wen Ze.

Only AI services. No broad shared domains (no bing.com, googleapis.com, gstatic.com, auth0.com, stripe.com, sentry.io). Those would hijack unrelated traffic.

## Files

Like blackmatrix7/ios_rule_script, one list per app, same domains:

- `rule/Surge/AI.list`
- `rule/Loon/AI.list`
- `rule/Shadowrocket/AI.list`

Surge, Loon and Shadowrocket use almost the same format, so the three files are the same domains. The only difference: Surge keeps the Gemini `URL-REGEX` redirect rule, Loon / Shadowrocket drop it (not reliable in their remote lists). Gemini itself is still covered.

## Use

Surge, in `[Rule]`:

```
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/surge-rules@main/rule/Surge/AI.list,美国
```

Loon, add as Remote Rule:

```
https://cdn.jsdelivr.net/gh/zwz0607/surge-rules@main/rule/Loon/AI.list
```

Shadowrocket, in `[Rule]`:

```
RULE-SET,https://cdn.jsdelivr.net/gh/zwz0607/surge-rules@main/rule/Shadowrocket/AI.list,PROXY
```

Replace the policy name (美国 / PROXY) with your own policy group name.

## Update

Edit the list, push, refresh the rule in the app. No need to re-add the link.
