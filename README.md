# pescms
Open the pescms login interface, enter the user name and password, capture the package, obtain the "back_url" parameter, 
![image](https://github.com/xuechengen/pescms/blob/main/3.png)
splice the parameters, and enter the code after the parameters for testing, http://XXXX/?m=Login&a=index&back_url=%22%3E%3Cscript%3Ealert(1);% 3C / script% 3E, XSS vulnerability is found.![image](https://github.com/xuechengen/pescms/blob/main/1.png)
By checking the source code, "back_url" is not filtered
![image](https://github.com/xuechengen/pescms/blob/main/2.png)
