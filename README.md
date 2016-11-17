# IS2545 DELIVERABLE 5: Security Test
### Jiawei Xu (jix20) and Tong Wei (tow6)

In this project, the security test was performed on a Windows 10 laptop with a Linux Virtual Machine: Oracle VM VirtualBox. The testing tools are Kali (https://www.kali.org/) which is a powerful testing tools package. This tools package can only be running on the Unix/Linux operating systems.
</br><br>
We have tested 3 websites choosing from the https://techguile.wordpress.com/2012/11/25/list-of-demo-websites-of-security-testing-purpose/,<br>
<li>http://demo.testfire.net/ , 
<li>http://zero.webappsecurity.com ,
<li>http://www.webscantest.com/.
#### Overall we have found <strong>11 vulnerabilities</strong> for these three websites:<br>
<br>
## 1. Website 1: http:// Demo.testfire.net
In this test, we applied Nikto, which is a website vulnerability scanner tool, to scan the vulnerability of the website1. The following figure shows the overall scan results and possible vulneralibity.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-1.png" width="600">

#### In this test, <strong>five vulnerabilities</strong> were found:<br>

<li>The directory, /bank, which is visible to unauthorized user. It violates Confidentiality, and interception can exploit this vulnerability. People can just use the url to get these private files. Usually the attacks exploit this vulnerability passively. And a lot of data will be lost due to the vulnerability. The development team need to rectify the code to make some update, in order to keep the directories invisible to the unauthorized users. Also, once those files are being downloaded, the system should be verifying the user identity. And after optimizing the relevant code, the developer also need to use the Nikto to make the test again.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-2.png" width="400">

<li>The directory, /pr, which is visible to unauthorized user. Just the same as the first vulnerability, it violates Confidentiality, and interception can exploit this vulnerability. People can just use the url to get these private files. Usually the attacks exploit this vulnerability passively. And a lot of data will be lost due to the vulnerability. For example, the Q3_earnings generally cannot be disclosed. The development team need to rectify the code to make some update, in order to keep the directories invisible to the unauthorized users. When the developers finish updating, they need to test it again.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-3.png" width="400">

<li>The file community annualreport.pdf, which is readable for unauthorized users. It violates Confidentiality. And interception can exploit this vulnerability. People can just use the url to get the private files. Usually the attacks exploit this vulnerability passively. And this important data will be lost due to the vulnerability. The development team need to rectify the code to make the update, in order to keep this files invisible to the unauthorized users. When the developers finish updating, they need to test it again.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-4.png" width="400">

<li>The confidential draft, Draft.rtf, which can be downloaded and read by unauthorized users.  It violates Confidentiality. And interception can exploit this vulnerability. People can just use the url to get the private files. Usually the attacks exploit this vulnerability passively. And this important data will be lost due to the vulnerability. We can see that this files have given us a caution that it is a confidential draft, so it shouldn’t be accessible to the unauthorized users. The development team need to rectify the code to make the update, in order to keep this files invisible to the unauthorized users. When the developers finish updating, they need to test it again. When this files need to be downloaded, the system should verify the user identity.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-5.png" width="400">

<li>The confidential document, Q3_earnings.rtf, which can be downloaded and read by unauthorized users.  It violates Confidentiality. And interception can exploit this vulnerability. People can just use the url to get the private files. Usually the attacks exploit this vulnerability passively. And this important data will be lost due to the vulnerability. The development team need to rectify the code to make the update, in order to keep this files invisible to the unauthorized users. When the developers finish updating, they need to test it again.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/1-6.png" width="400">
<br>

## 2. Website 2: http://zero.webappsecurity.com
In this test, we also applied Nikto to scan the vulnerability of the website1. The following figure shows the overall scan results and possible vulneralibity.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-1.png" width="600">


#### In this test, <strong>Three vulnerabilities</strong> were found:<br>


<li>The directory, /admin, is visible to unauthorized user. It violates Confidentiality. And interruption, interception and modification can exploit this vulnerability. People can just use this url to get accessed to this page without any verification. Usually the attacks exploit this vulnerability actively. And the development team need to rectify the code to make the update, in order to make this page not accessible to the unauthorized users. When the developers finish updating, they need to test it again.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-2.png" width="400">

<li>The confidential information of users, such as user name, password, and SSN are readable by unauthorized users. It extremely violates Confidentiality.  And interruption and interception can exploit this vulnerability. People can just use this url to get accessed to this page without any verification. Usually the attacks exploit this vulnerability actively. And the development team need to rectify the code to make the update, in order to make this page not accessible to the unauthorized users. When the developers finish updating, they need to test it again to make sure it is secure.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-3.png" width="600">

<li>The confidential information of Currencies, is writable to unauthorized users:(We have Exploiting Vulnerability by add the last line, see the following snapshot). It violates Confidentiality and Integrity. And interruption, interception and modification can exploit this vulnerability. People can just use this url to get accessed to this page to get users’ private information. Usually the attacks exploit this vulnerability actively. And the development team need to rectify the code to make the update, in order to make this page not accessible to the unauthorized users. When the developers finish updating, they need to test it again to make sure it is secure.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/2-4.png" width="600">

<br>
## 3. Website 3: http://www.webscantest.com/
In this test, we also applied Nikto to scan the vulnerability of the website1. The following figure shows the overall scan results and possible vulneralibity.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-1.png" width="600">

#### In this test, <strong>Three vulnerabilities</strong> were found:<br>

<li>The confidential file, robots.txt, containing 4 entries, which is visible to unauthorized user. It violates Confidentiality. And interception can exploit this vulnerability. People can just use the url to get the private files. Usually the attacks exploit this vulnerability passively. And this important data will be lost due to the vulnerability. The development team need to rectify the code to make the update in order to keep this files invisible to the unauthorized users. When the developers finish updating, they need to test it again and to make sure it is secure.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-2.png" width="400">

<li>The directory, /osrun, is visible to the unauthorized user. It violates Confidentiality. It is vulnerable to cmd inject. And modification can exploit this vulnerability. People can just use the url to get accessed to this page. Usually the attacks exploit this vulnerability actively. The development team need to rectify the code to make the update, in order to keep the page not accessible to the unauthorized users. When the developers finish updating, they need to test it again and to make sure it is secure.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-3.png" width="600">

<li>The directory, /cal_endar, is visible to unauthorized users. It violates Confidentiality. The users’ appointments are all readable to unauthorized users. And interception can exploit this vulnerability. People can just use this url to get accessed to this page without any verification. Usually the attacks exploit this vulnerability actively. And the development team need to rectify the code to make the update, in order to make this page not accessible to the unauthorized users. When the developers finish updating, they need to test it again to make sure it is secure.<br>
<img src="https://github.com/jiaweixu/Security-Test/blob/master/material/3-4.png" width="600">
