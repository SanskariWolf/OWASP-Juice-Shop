| [[Missing Encoding]] | Retrieve the photo of Bjoern’s cat in "melee combat-mode". | ⭐   |
| -------------------- | ---------------------------------------------------------- | --- |

In `/photo-wall` endpoint, the the first image is broken
![](../Images/Pasted%20image%2020260415085342.png)

![](../Images/Pasted%20image%2020260415085444.png)

the image path
`assets/public/images/uploads/ᓚᘏᗢ-#zatschi-#whoneedsfourlegs-1572600969477.jpg`

The letter `#` should be URL encoded as in HTML it is consider as HTML anchor so to consider it as a path element we need it to be URL encoded.

Thus `#` should be written as `%23`
![](../Images/Pasted%20image%2020260415085724.png)

And completed
