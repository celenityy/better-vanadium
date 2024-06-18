# better-vanadium

My recommendations for the ultimate configuration of the [Vanadium](https://github.com/GrapheneOS/Vanadium) & [Mulch](https://gitlab.com/divested-mobile/mulch) Browsers :)

**NOTE:** This project can be found on both [Codeberg](https://codeberg.org/Magnesium1062/better-vanadium), which will act as the main & preferred way to contribute, and [GitHub](https://github.com/Retold3202/better-vanadium).

# Search engine

**Search engine** -> `DuckDuckGo` ✅

# Password Manager

**Save passwords** -> ❌ *(You should not save info in your browser like this for security reasons, use a dedicated password manager like Bitwarden or Proton Pass instead)*

**Auto Sign-in** -> ❌

# Payment methods

**Save and fill payment methods** -> ❌ *(You should not save info in your browser like this for security reasons, use a dedicated password manager like Bitwarden or Proton Pass instead)*

**Manually verify every time you pay using autofill** -> ✅

# Addresses and more

**Save and fill addresses** -> ❌ *(You should not save info in your browser like this for security reasons, use a dedicated password manager like Bitwarden or Proton Pass instead)*

# Autofill Options

**Autofill Options** -> `Use other providers` ✅

# Privacy and security

Privacy -> **Third-party cookies** -> `Block third-party cookies` ✅ *(Should be default)*

Privacy -> Third-party cookies -> Block third-party cookies -> **Allow related sites to see your activity in the group** -> ❌

Privacy -> **Close tabs on exit** -> ✅

Privacy -> **Cross-origin referrer policy** -> `Disable cross-origin referrer` ✅ *(If this causes you any issues, you could also set this to `Reduce cross-origin referrer`)*

Privacy -> **Improve search suggestions** -> ❌

Privacy -> **WebRTC IP handling policy** -> `Disable non-proxied UDP` *(Don't set this if you have to call on the web through services like Discord & Zoom)*

Security -> **Safe Browsing** -> `No protection (not recommended)` ❌ *(On Android, Safe Browsing requires Google Play Services and as such is proprietary and questionable. As long as you have other protection in place (See `secure DNS` & `Additional recommendations` below), then I don't think its worth using here)*

Security -> **Always use secure connections** -> ✅

Security -> **Use secure DNS** -> ✅

Security -> Use secure DNS -> Choose another provider -> **Custom** -> Pick a private, secure, & reputable DNS provider of your choice, I would recommend setting up your own [NextDNS](https://nextdns.io) configuration if you are able to (See my recommendations for NextDNS [here](https://codeberg.org/Magnesium1062/nextdns-settings), otherwise I would recommend [Quad9](https://quad9.net/): `https://dns.quad9.net/dns-query` *(Even if you have a private/secure DNS provider set on your OS/network level, make sure to still set it here too like this, so that you can take advantage of [Encrypted Client Hello](https://blog.cloudflare.com/announcing-encrypted-client-hello))*

Security -> **Access payment methods** -> ❌

# Notifications

General -> **All "General Notifications** -> ✅

General -> **Browser** -> ❌

General -> **Completed downloads** -> ✅

General -> **Active downloads** -> ✅

General -> **Incognito** -> ✅

General -> **Playing media** -> ✅

# Toolbar shortcut

**Toolbar shortcut** -> `New tab`

# Accessibility

**Force enable zoom** -> ✅

**Simplified view for web pages** -> ✅

# Site settings

Permissions -> **Location** -> `Blocked` ❌ 

Permissions -> **Camera** -> `Blocked` ❌ *(Obviously don't set if you use sites that need camera access, but you can still set exceptions for sites if needed*)

Permissions -> **Microphone** -> `Blocked` ❌ *(Obviously don't set if you use sites that need microphone access, but you can still set exceptions for sites if needed*)

Permissions -> **Notifications** -> `Blocked` ❌

Permissions -> **Embedded content** -> `Blocked` ❌

Permissions -> **Motion sensors** -> `Blocked` ❌

Permissions -> **NFC devices** -> `Blocked` ❌

Permissions -> **USB** -> `Blocked` ❌

Permissions -> **Clipboard** -> `Blocked from reading clipboard` ❌

Permissions -> **Virtual reality** -> `Blocked` ❌

Permissions -> **Augmented reality** -> `Blocked` ❌

Permissions -> **Your device use** -> `Blocked` ❌

Content -> **JavaScript** -> `Blocked` ❌ *(This **will** cause breakage, but it heavily improves privacy & security, so I'd recommend blocking it if possible and if you're willing to re-enable JavaScript on sites that need it)*

Content -> **JavaScript JIT** -> `Blocked` ❌ *(Should be default)*

Content -> **Pop-ups and redirects** -> `Blocked` ❌ *(Should be default)*

Content -> **Ads** -> `Blocked` ❌

Content -> **Protected content** -> `Blocked` ❌ - https://www.eff.org/deeplinks/2017/10/drms-dead-canary-how-we-just-lost-web-what-we-learned-it-and-what-we-need-do-next

Content -> **Auto-verify** -> `Blocked` ❌

Content -> **Dark theme for sites** -> `On` ✅ *(See `chrome://flags` below)*

Content -> **Background sync** -> `Blocked` ❌

# Downloads

**Ask where to save files** -> ✅

**Automatically open PDFs** -> ❌

# chrome://flags

`#android-open-pdf-inline` -> `Enabled`

`#darken-websites-checkbox-in-themes-setting` -> `Enabled` *(This will allow you to toggle `Dark theme for sites` under `Site settings` above)*

`#enable-parallel-downloading` -> `Enabled`

`sanitizer-api` -> `Enabled`

# Additional recommendations

* Use a (reputable) VPN. I would recommend either [Mullvad](https://mullvad.net/) or [ProtonVPN](https://protonvpn.com/).

* Use a (reputable) anti-virus if possible, such as [Hypatia](https://f-droid.org/packages/us.spotco.malwarescanner/). **NOTE:** You should install Hypatia through the [DivestOS Official Repo](https://divestos.org/fdroid/official/?fingerprint=E4BE8D6ABFA4D9D4FEEF03CDDA7FF62A73FD64B75566F6DD4E5E577550BE8467) instead of F-Droid's main repo, as it will allow you to receive quicker updates directly from the developer. It's also recommended to use [F-Droid Basic](https://f-droid.org/en/packages/org.fdroid.basic/) as your F-Droid client of choice.