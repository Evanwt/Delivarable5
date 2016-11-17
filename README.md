# IS2545 DELIVERABLE 5: Security Test
## Jiawei XU (jix20) & Tong Wei (tow6)


In this project, the security test was performed on a Windows 10 laptop with a Linux Virtual Machine: Oracle VM VirtualBox. The testing tools are Kali (https://www.kali.org/) which is a powerful testing tools, it can only be running on the Unix/Linux operating systems.
</br>
We are going to test 3 websites choosing from the https://techguile.wordpress.com/2012/11/25/list-of-demo-websites-of-security-testing-purpose/,<br>
<li>http://demo.testfire.net/ , 
<li>http://zero.webappsecurity.com ,
<li>http://www.webscantest.com/.



### Website 1: http:// Demo.testfire.net</br>
In this test, we applied Nikto, which is a website vulnerability scanner tool, to scan the vulnerability of the website1. The following figure shows the overall scan results and possible vulneralibity.</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-1.png" width="600">

In this test,five vulnerabilities were found:<br>
1. The directory, /bank, which is visible to unauthorized user. It violates Confidentiality, and interception can exploit this vulnerability. People can just use the url to get these private files. Usually the attacks exploit this vulnerability passively. And a lot of data will be lost due to the vulnerability. The development team need to rectify the code to make some update, in order to keep the directories invisible to the unauthorized users. Also, once those files are being downloaded, the system should be verifying the user identity. And after optimizing the relevant code, the developer also need to use the Nikto to make the test again.</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-2.png" width="400">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-3.png" width="400">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-4.png" width="400">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-5.png" width="400">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-6.png" width="400">


### 2.  Security Testing on website 2:</br>
The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-1.png" width="600">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-2.png" width="400">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-3.png" width="600">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-4.png" width="600">


### 3.  Security Testing on website 3:</br>
The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-1.png" width="600">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-2.png" width="400">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-3.png" width="600">

The following figure shows M:</br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-4.png" width="600">
