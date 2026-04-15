| [[Repetitive Registration]] | Follow the DRY principle while registering a user.                                          | ⭐          |
| --------------------------- | ------------------------------------------------------------------------------------------- | ---------- |
DRY principle
(D)Don't (R)Repear (Y)Yourself

While registration, the password check validation is not done properly
![](../Images/Pasted%20image%2020260415091643.png)
In the function, Repeat password column is checked only once when the password is being typed, Once typed, the used can change the passControl dialog and there is no check for Repeat Password to match the origianal one.
And that's the flaw.


![](../Images/Pasted%20image%2020260415091133.png)