Ok so client-side script is main.js itself,
searching for the credentials and found those with term `testing` itself.
![](../Images/Pasted%20image%2020260415183307.png)
```
└─$ js-beautify main.js | grep "testing"
            testingUsername = "testing@juice-sh.op";
            testingPassword = "IamUsedForTesting";
```

![](../Images/Pasted%20image%2020260415183449.png)
Solved
