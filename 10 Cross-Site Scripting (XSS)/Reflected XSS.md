| [[Reflected XSS]] | Perform a _reflected_ XSS attack with ``<iframe src="javascript:alert(`xss``)">`. | ⭐⭐  |
| ----------------- | --------------------------------------------------------------------------------- | --- |
|                   |                                                                                   |     |
Fiddling with the page, i noticed that many things are getting reflected back, one of the peculiar that took my attention was  Address and Order history

Over Order History, ID of the order is getting reflected back at the page,
![](../Images/Pasted%20image%2020260415102030.png)

Therefore, I went with Reflected XSS payload and boom the vulnerability was there.
![](../Images/Pasted%20image%2020260415102018.png)
Thus solved
