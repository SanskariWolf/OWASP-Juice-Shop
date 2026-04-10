### Setting up the lab

I am using Packed Distribution Steps to install it over my system.

![](Images/Pasted%20image%2020260410080001.png)

As my system is linux using node vesion 20 (you can use `node -v` to check the node version in your terminal)
![](Images/Pasted%20image%2020260410080214.png)

Following the steps ahead, i.e. unpacking and getting inside the folder and doing npm start
![](Images/Pasted%20image%2020260410080343.png)

and there i go, i have the back-end listening and front-end is there on the port listening on port 3000 as stated in the installation steps.

## Summary

Owasp-Juice Shop is being tested for all the vulnerabilities it have.


## Challenges Categories

![](Images/Pasted%20image%2020260410082332.png)

### Sunny Day Scenario

Link : `http://localhost:3000/#/`
![](Images/Pasted%20image%2020260410084803.png)

Pages
- Accessible Without Login
	1. `localhost/#/contact`
		![](Images/Pasted%20image%2020260410084823.png)
	2. `localhost:3000/#/about`
		![](Images/Pasted%20image%2020260410084841.png)
	3. `localhost:3000/#/photo-wall`
		![](Images/Pasted%20image%2020260410084858.png)
	4. `localhost:3000/#/login`
		![](Images/Pasted%20image%2020260410084917.png)
	5. `localhost:3000/#/register`
		![](Images/Pasted%20image%2020260410084932.png)
- Accessible After Login
	1. `localhost:3000/#/` 
		![](Images/Pasted%20image%2020260410085115.png)
	2. `localhost:3000/#/complain`
		![](Images/Pasted%20image%2020260410085211.png)
	3. `localhost:3000/#/chatbot`
		![](Images/Pasted%20image%2020260410085250.png)
	4. `localhost:3000/#/deluxe-membership`
		![](Images/Pasted%20image%2020260410085338.png)
	5. `localhost:3000/#/basket`
		![](Images/Pasted%20image%2020260410085431.png)

## Doing manually mapping of endpoints is tiring, i used zaproxy ajax spider 

It Solved a few 1-start challenges
- Solved 1-star directoryListingChallenge (Confidential Document)
![](Images/Pasted%20image%2020260410090150.png)
	- In About Us there is link embed which leads to `localhost:3000/#/ftp/legal.md`. Giving us the flag. It can be accessed other way too, there is a `localhost:3000/robots.txt` page that is made generally for web crawlers, and there the `localhost:3000/ftp` endpoint is noted. we can directly go to `localhost:3000/ftp` giving us many more files.
		![](Images/Pasted%20image%2020260410091551.png)
		![](Images/Pasted%20image%2020260410091814.png)


![](Images/Pasted%20image%2020260410121514.png)