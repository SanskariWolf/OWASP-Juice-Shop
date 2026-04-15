| [[Outdated Allowlist]] | Let us redirect you to one of our crypto currency addresses which are not promoted any longer. | ⭐          |
| ---------------------- | ---------------------------------------------------------------------------------------------- | ---------- |
since it's about redirecting,
we can search in main.js for redirecting links
![](../Images/Pasted%20image%2020260415090323.png)

```
└─$ js-beautify main.js | grep "redirect" 
                    ["mat-list-item", "", "href", "./redirect?to=https://github.com/juice-shop/juice-shop", "aria-label", "Go to OWASP Juice Shop GitHub page"],
            redirectUri = "";
                e ? (this.user = {}, this.user.email = e, this.rememberMe.setValue(!0)) : this.rememberMe.setValue(!1), this.redirectUri = `${this.windowRefService.nativeWindow.location.protocol}//${this.windowRefService.nativeWindow.location.host}`, this.configurationService.getApplicationConfiguration().subscribe({
                            let a = i.application.googleOauth.authorizedRedirects.find(r => r.uri === this.redirectUri);
                            a ? (this.oauthUnavailable = !1, this.redirectUri = a.proxy ? a.proxy : a.uri) : (this.oauthUnavailable = !0, console.log(this.redirectUri + " is not an authorized redirect URI for this application."))
                this.windowRefService.nativeWindow.location.replace(`${cR}?client_id=${this.clientId}&response_type=token&scope=email&redirect_uri=${this.redirectUri}`)
                        url: "./redirect?to=https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm",
                        url: "./redirect?to=https://explorer.dash.org/address/Xr556RzuwX6hg5EGpkybbv5RanJoZN17kW",
                        url: "./redirect?to=https://etherscan.io/address/0x0f933ab9fcaaa782d0279c300d73750e1311eae6",
                    ["href", "./redirect?to=http://shop.spreadshirt.com/juiceshop"],
                    ["href", "./redirect?to=http://shop.spreadshirt.de/juiceshop"],
                    ["href", "./redirect?to=https://www.stickeryou.com/products/owasp-juice-shop/794"],
                    ["href", "./redirect?to=http://leanpub.com/juice-shop"],
```

So we have that redirect link
url: "./redirect?to=https://blockchain.info/address/1AbKfgvw9psQ41NbLi8kufDQTezwG8DRZm"

Let's go and trigger this to solve the challenge
![](../Images/Pasted%20image%2020260415090611.png)

Solved 