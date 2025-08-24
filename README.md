# Malvertising
A Web Security Case Study in Malvertising and Adversarial UX

_This repo documents a personal cybersecurity investigation into malvertising and adversarial UX design on freemium cartoon streaming platforms._

## 🌐 Project Scope

- Analyze how malvertising chains manipulate browser focus and user behavior.
- Track known suspicious domains (e.g. `junior-shine[.]com`) and their network behavior.
- Test hardened browser/VPN/VM setups to reduce exposure.
- Reflect on the socioeconomic implications of “free” platforms that penalize non-paying users with potential malware.

## 🔍 Skills Demonstrated

- Web application and client-side threat modeling
- DNS and network monitoring (DevTools, Wireshark)
- Secure VM + browser setup
- Ethical reflection on digital access and exploitation

## 🛡️ Tools Used

- Chrome DevTools
- Malwarebytes + AV logs
- VirtualBox
- uBlock Origin, NoScript
- Burp Suite Community Edition

---

This project is ongoing and intended as both a technical portfolio piece and a reflection on digital safety for economically marginalized users.

💥 The Core Ethical Dilemma:

**“Is it justifiable to expose non-paying users to malware?”**

**Short answer:**
Hell no.
**Longer answer:**
It's predatory as hell, and it reflects how capitalism weaponizes access to art and entertainment.

🧠 Let’s Break It Down Like a Hacker AND a Human:

🩸 1. Economic Exploitation ≠ Informed Consent

These sites operate on the premise that if you’re not paying, your data, your device, or your attention becomes the currency. But:

Most users don’t realize how deeply they’re being exposed (drive-by downloads, forced redirects, focus stealing, exploit kits).

Even if they do, the choice is between entertainment and danger—not safety and danger.

That’s not a “fair trade.” That’s coercion. And you felt that—because even with an AV and an adblocker, you knew this shit wasn’t safe. You’re not being paranoid. You’re being perceptive.

⚠️ 2. Technical Truth: The Attack Surface is Massive

Sites like this often serve:

Obfuscated JavaScript that builds fake redirects

Hidden iframes to other domains like junior-shine[.]com (which might do fingerprinting or attempt XSS)

Clickjacking traps ("Click to Play" buttons that open multiple tabs behind the scenes)

Exploit kits that detect outdated browser plugins, PDF readers, or Java

Even WITH:

uBlock Origin

Privacy-focused browsers (Brave, Firefox containers)

Real-time AV

…you're still threading a needle.

🧼 3. User Reality: You Deserve Safety, Even if You Can’t Pay

This is where ethics hits the hardest:

You’re not wrong to stream your favorite animated show to survive a hard night.
You’re not wrong to keep your world calm through memorable, lovable characters from shows you grew up with.
You’re not wrong to seek a little peace or laughter without a subscription.

What’s wrong is that “free” now comes with a built-in exploit pipeline. Because:

Capitalism’s logic is: monetize the user either way.

If you can't pay cash, you’ll pay in device resources, personal data, or malvertising exposure.

That’s not just shady—it’s inhumane.

🧰 Practical Tips (because survival still matters)

✅ Yes, Use a VM if You Can

Spin up a light Linux VM (like Ubuntu) with:

A hardened browser (Brave, Firefox + containers)

uBlock Origin + NoScript

DNS filtering (like NextDNS, or even Cloudflare’s 1.1.1.2 for malware protection)

That way, if something does hit you, it stays in the sandbox.

✅ Use a Dedicated Profile or Disposable Container

Short of a VM:

New Chrome/Firefox profile JUST for these sites

No saved passwords

No synced extensions

Clear cache on exit

✅ Track Domains in DevTools

Next time you're watching, pop open DevTools > Network tab and log suspicious domains.
You’ll start to see patterns:

What domains redirect you?

What causes a cursor blink or tab switch?

That becomes evidence—and training.

Some of the initial goals with this repo include: 

✅ 1. Real-World Application of Cyber Concepts

✅ 2. Web App Security + Client-Side Threat Awareness

Malvertising lives in the intersection of:

Web app security (JS injection, iframe abuse)

User-side vulnerabilities (browser APIs, DNS resolution)

Cloud delivery models (ad CDN abuse, traffic obfuscation)

Including this project shows understanding of how malicious payloads actually travel over the web and impact end-users.

✅ 3. Good Signal for Red Team + Cloud Focus

Potential lab and TryHackMe labs can help with demonstrating:

Exploit chain analysis

Threat actor behavior emulation

User behavior modeling

And even cloud security via DNS/ad delivery implications


