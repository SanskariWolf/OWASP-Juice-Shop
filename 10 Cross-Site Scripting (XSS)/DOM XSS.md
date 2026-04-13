| [DOM XSS](https://owasp.org/www-community/attacks/DOM_Based_XSS) | Perform a _DOM_ XSS attack with ``<iframe src="javascript:alert(`xss``)">`. | ⭐   |
| ---------------------------------------------------------------- | --------------------------------------------------------------------------- | --- |
DOM-based Cross-Site Scripting is the de-facto name for XSS bugs which are the result of active browser-side content on a page, typically JavaScript, obtaining user input and then doing something unsafe with it which leads to execution of injected code.

The DOM, or Document Object Model, is the structural format used to represent documents in a browser. The DOM enables dynamic scripts such as JavaScript to reference components of the document such as a form field or a session cookie. The DOM is also used by the browser for security - for example to limit scripts on different domains from obtaining session cookies for other domains. A DOM-based XSS vulnerability may occur when active content, such as a JavaScript function, is modified by a specially crafted request such that a DOM element that can be controlled by an attacker.

Putting the value `<iframe src="javascript:alert(`xss`)">` in Search Field and thus get the answer. 

![](../Images/Pasted%20image%2020260413112824.png)
