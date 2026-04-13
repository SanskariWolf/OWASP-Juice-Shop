# Finding the Score Board (Challenge 01)
If we parse through the initial guided instruction, we can see that it says to pass through the JS code,
So let's go though it,
we have three JS files _(Others are intermediate JS generated for functioning, (chunk ones))_
```
main.js
script.js
polyfills.js
```

Let's hunt over `main.js`
- One thing we know is that Owasp Juice Shop is build over Angular framework.
- And Angular have this pre-defined way of routing application i.e. `routes`
Let's search for the work route and map all the paths,

so instead of liking to use `Ctrl+F`, I like command line tools more `grep`
I loaded main.js in my locally by `wgtet http://localhost:3000/main.js`
After loaded the code was is prettified format, thus i used `js-beaurify` and use `grep "route"` but there were many random scribble among which i was able to identify the minimal version that could be used to aid the search and reduce the gibberish `grep "routerLink\", \""`

![](Images/Pasted%20image%2020260413113753.png)

So i was able to identify that the path to the score board is `/score-board`

![](Images/Pasted%20image%2020260413105147.png)

---
We are going to map challenges in chapter-wise manner,

1. [[03 Injection/Injection]]
2. [[04 Broken Authentication/Broken Authentication]]
3. [[05 Sensitive Data Exposure/Sensitive Data Exposure]]
4. [[XML External Entities(XXE)]]
5. [[Improper Input Validation]]
6. [[Broken Access Control]]
7. [[09 Security Misconfiguration/Security Misconfiguration]]
8. [[10 Cross-Site Scripting (XSS)/Cross-Site Scripting (XSS)]]
9. [[Insecure Deserialization]]
10. [[Vulnerable Components]]
11. [[Security though Obscurity]]
12. [[Unvalidated Redirects]]
13. [[Broken Anti-Automation]]
14. [[Cryptographic Issues]]
15. [[17 Observability Failures/Observability Failures]]
16. [[18 Miscellaneois/Miscellaneous]]