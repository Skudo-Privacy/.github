<div align="center">

<img src="https://raw.githubusercontent.com/Skudo-Privacy/.github/main/profile/assets/icon.png" width="112" height="112" alt="Skudo" />

<br />

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Skudo-Privacy/.github/main/profile/assets/wordmark-light.png">
  <img src="https://raw.githubusercontent.com/Skudo-Privacy/.github/main/profile/assets/wordmark-dark.png" height="34" alt="Skudo" />
</picture>

### Every site gets its own email address. Your real one stays yours.

[![Website](https://img.shields.io/badge/website-skudo.org-0f5e56)](https://skudo.org)
[![Free](https://img.shields.io/badge/price-free-0f5e56)](https://skudo.org/donate/)
[![No ads](https://img.shields.io/badge/ads%20%26%20profiling-none-0f5e56)](https://skudo.org/legal/privacy/)
[![Warrant canary](https://img.shields.io/badge/warrant%20canary-signed%20every%2030%20days-0f5e56)](https://skudo.org/transparency/)
[![Extension](https://img.shields.io/badge/extension-Firefox%20%C2%B7%20Chrome-0f5e56)](https://github.com/Skudo-Privacy/skudo-extension)

**[Create a free account](https://app.skudo.org/register)** &nbsp;·&nbsp; [Security architecture](https://skudo.org/security/architecture/) &nbsp;·&nbsp; [Transparency](https://skudo.org/transparency/)

</div>

---

Skudo gives each site you sign up to a unique alias. Mail sent to it reaches the inbox you already use, and you can reply from the alias without your real address ever appearing in the headers. When a site leaks your address or sells it, you know exactly who did it, and you switch off that one alias. Every other address keeps working.

Privacy is not a feature we added on top. It is the reason Skudo exists, and the whole service is built around it.

## Privacy, by design

| Protection | In practice |
|---|---|
| **A sealed mapping** | The address an alias forwards to is encrypted with its own key and found through a blind index. A copy of our database alone would not tell anyone where your mail goes. Notes and display names are encrypted too. |
| **Relayed, not archived** | In the normal case a message goes straight from the incoming connection to the outgoing one, and nothing is archived. The mail server log is read and cleared every five minutes. |
| **Your key, if you want it** | Upload an OpenPGP key and your mail is encrypted to it before it leaves Skudo. |
| **Trackers stripped** | Tracking pixels and tracking parameters in links (utm_campaign, fbclid and the rest) are removed from forwarded mail. On by default. |
| **No ads, no profiling** | We do not sell data. The website loads no third-party scripts, fonts or analytics, and the build fails if a third-party request slips in. |
| **One address per site** | Find out who leaked you, block a single alias, route different aliases to different inboxes, and leave everything else untouched. |

## Proof, not promises

<table>
<tr>
<td width="50%" valign="top">

**A signed warrant canary**<br />
Renewed by a person every 30 days, signed with a key published in advance, and anchored to the latest Bitcoin block so it cannot be signed early.

</td>
<td width="50%" valign="top">

**A transparency log**<br />
Built as a Merkle tree, with a signed root, so entries can be checked and not just read.

</td>
</tr>
<tr>
<td width="50%" valign="top">

**A quarterly transparency report**<br />
Six figures fixed in advance: orders received, orders asking for an identity, addresses decrypted, accounts involved, requests refused and emergency disclosures. Due within 30 days of each quarter's end.

</td>
<td width="50%" valign="top">

**Published legal process**<br />
How every legal request is reviewed, refused and counted is written down in [legal requests](https://skudo.org/legal/requests/).

</td>
</tr>
</table>

## Everywhere you type an email

- **Browser extension** for Firefox and Chrome, with the source on GitHub: [skudo-extension](https://github.com/Skudo-Privacy/skudo-extension)
- **Your own domain**, or Skudo's, and your existing inbox: Gmail, Outlook, iCloud or your own server
- **Bitwarden**: generate an alias straight from the password manager

## Based in Italy, under GDPR

Skudo is operated from Italy and is subject to the GDPR. The [privacy policy](https://skudo.org/legal/privacy/) says exactly what is kept and for how long. It is funded by voluntary donations, about 90 euros a month, never by advertising: [donate](https://skudo.org/donate/).

---

<div align="center">

[skudo.org](https://skudo.org) &nbsp;·&nbsp; [Blog](https://skudo.org/blog/) &nbsp;·&nbsp; [Report a vulnerability](https://skudo.org/security/disclosure/) &nbsp;·&nbsp; [Donate](https://skudo.org/donate/)

</div>
