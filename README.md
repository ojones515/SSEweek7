# Project 7 - WordPress Pentesting

Time spent: **X** hours spent in total

> Objective: Find, analyze, recreate, and document **five vulnerabilities** affecting an old version of WordPress

## Pentesting Report

1. Authenticated Cross-Site Scripting (XSS) via Media File Metadata
  - [ ] Summary: 
                The admin uploads what appears to be an mp3 but is actually a link to another page
    - Vulnerability types: XSS
    - Tested in version: 4.2
    - Fixed in version: 4.2.13
  - [ ] GIF Walkthrough:
  
  <a href="https://i.imgur.com/7eWlxFU.gif"><img src="https://i.imgur.com/7eWlxFU.gif" title='Video Walkthrough' width='' alt='Video Walkthrough' /></a>
  
  - [ ] Steps to recreate: 
                      - 1. Download fake mp3 file from https://sumofpwn.nl/advisory/SFY20160742/xss.mp3
                      - 2. Give to admin of site
                      - 3. Have Admin upload and post to a page on the site
                      - 4. When clicked, any user will be sent to another website
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/branches/4.2/src/wp-admin/includes/media.php)
    
2. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)
3. (Required) Vulnerability Name or ID
  - [ ] Summary: 
    - Vulnerability types:
    - Tested in version:
    - Fixed in version: 
  - [ ] GIF Walkthrough: 
  - [ ] Steps to recreate: 
  - [ ] Affected source code:
    - [Link 1](https://core.trac.wordpress.org/browser/tags/version/src/source_file.php)


## Assets

xss.mp3 (https://sumofpwn.nl/advisory/SFY20160742/xss.mp3)

## Resources

- [WordPress Source Browser](https://core.trac.wordpress.org/browser/)
- [WordPress Developer Reference](https://developer.wordpress.org/reference/)
- https://sumofpwn.nl/advisory/2016/wordpress_audio_playlist_functionality_is_affected_by_cross_site_scripting.html

GIFs created with [LiceCap](http://www.cockos.com/licecap/).

## Notes

No Notes at this time.

## License

    Copyright [2018] [Christopher Jones]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
