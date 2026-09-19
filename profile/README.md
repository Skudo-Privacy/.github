# Skudo

Skudo gives every site its own email address. Mail sent to an alias reaches the inbox you already use, and you can reply from the alias without your real address ever appearing in the headers. If a site leaks or sells its list, you know who did it, and you switch off that one address without touching the others.

It is free, funded by voluntary donations, and built around one idea: an alias service should know as little about you as it can, and be honest about the rest.

## How the privacy works

**The mapping is sealed.** The address an alias forwards to is encrypted with its own key, and looked up through a blind index. A copy of our database alone would not tell anyone where your mail goes. Notes and display names are encrypted as well.

**Your messages are not stored.** A message passes from the incoming connection to the outgoing one. The one exception is a destination that cannot be reached: the message waits in the mail queue on disk until it is delivered or expires. The mail server log is read and cleared every five minutes. If you upload an OpenPGP key, mail is encrypted to it before it leaves us.

**Trackers are stripped.** Tracking pixels and tracking parameters in links (utm_campaign, fbclid and friends) are removed from forwarded messages. It is a per-account setting, on by default, and it only touches what it can recognise with certainty.

**No ads, no profiling.** We do not sell data, and the website loads no third-party scripts, fonts or analytics. The build checks for third-party requests, so a stray one fails it.

## What we can and cannot protect you from

We would rather say it here than have you find it later. Skudo decrypts your forwarding address every time it delivers a message, so the key lives on our production machines, and with a valid legal order we could decrypt it. There is no second party to ask. We cannot protect you from traffic analysis on both sides, from the provider of your own inbox, from coercion aimed at you, or from us. No independent audit has been done yet. If one is commissioned, the report will be published in full.

## Verify, do not trust

- **A signed warrant canary**, renewed by a person every 30 days, signed with a key published in advance and anchored to the latest Bitcoin block, so it cannot be signed ahead of time.
- **A transparency log** built as a Merkle tree, with a signed and published root.
- **A quarterly transparency report** with six figures defined in advance: orders received, orders asking for an identity, addresses decrypted, accounts involved, requests refused and emergency disclosures. Each report is due within 30 days of the end of the quarter.
- **Published legal process:** how we review, refuse and count requests is written down in [legal requests](https://skudo.org/legal/requests/).
- **The browser extension is on GitHub**, source-available, so you can read what runs in your browser: [skudo-extension](https://github.com/Skudo-Privacy/skudo-extension).

## Who runs it

Skudo is operated by an individual in Italy, who is the GDPR data controller and answers to Italian courts. The details are in the [privacy policy](https://skudo.org/legal/privacy/).

## Read more

- [skudo.org](https://skudo.org)
- [Security architecture](https://skudo.org/security/architecture/): the full threat model, including what it does not cover
- [Transparency](https://skudo.org/transparency/): canary, log and reports
- [Vulnerability disclosure](https://skudo.org/security/disclosure/)
- [The blog](https://skudo.org/blog/)
- [Donate](https://skudo.org/donate/): the running cost is about 90 euros a month
