## 🔎 𝚒𝚗𝚍𝚎𝚟𝚒𝟶𝚞𝚜@𝙽𝚎𝚖𝚎𝚜𝚒𝚜:~$ 𝚠𝚑𝚘𝚊𝚖𝚒:
Offensive Security Researcher, Bug Bounty Hunter, Hacker, Malware Whisperer, OWASP Member, Hackfluencer, Speaker, and other words that end with -er.

![](black_cat_banner.gif)

**ɴᴏᴛ ᴀ ᴡᴇʙ ᴀᴘᴘ ᴇxᴏʀᴄɪꜱᴛ, ᴊᴜꜱᴛ ᴛʜᴇ ᴏɴᴇ ᴡʜᴏ ᴘᴏꜱꜱᴇꜱꜱᴇꜱ ᴛʜᴇᴍ.**

## 🏆 Achievements:
* [1st Hacker in Hackrate's Global Leaderbord](https://hckrt.com/Home/Leaderboard);
* [Top Contributor in Security Research for Teclib's GLPI 9.5.4 release](https://www.teclib-edition.com/en/glpi-9-5-4/);
* [Interviewed by Hackrate](https://elite.hckrt.com/hackers/indevi0us.html);
* [Interviewed by MyHackerTech (MHT)](https://myhackertech.com/blogs/news/interview-with-samuele-gugliotta-aka-0x3qt-or-xeqt).

## 📄 Public Writeups:
* [Full Account Takeover of ANY user via Insecure Direct Object Reference (IDOR) on reset password functionality](https://blog.hckrt.com/blog/thisclosed_1/)

## 🌐 Social Networks:
[![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/samuele-gugliotta) [![Reddit](https://img.shields.io/badge/Reddit-%23FF4500.svg?logo=Reddit&logoColor=white)](https://reddit.com/user/indevi0us) [![Twitter](https://img.shields.io/badge/Twitter-%231DA1F2.svg?logo=Twitter&logoColor=white)](https://twitter.com/indevi0us) [![Reddit](https://img.shields.io/badge/Twitch-6441a5?logo=twitch&logoColor=white)](https://www.twitch.tv/indevi0usTV) [![Instagram](https://img.shields.io/badge/Instagram-8a3ab9?logo=instagram)](https://instagram.com/indevi0us)

## 🔊 Published CVEs:
|    Date    |       CVE ID       | Description  |
|------------|--------------------|--------------|
|11/26/2020|[CVE-2020-27662](https://nvd.nist.gov/vuln/detail/CVE-2020-27663)|In GLPI before 9.5.3, ajax/comments.php has an Insecure Direct Object Reference (IDOR) vulnerability that allows an attacker to read data from any database table (e.g., glpi_tickets, glpi_users, etc.).|
|11/26/2020|[CVE-2020-27663](https://nvd.nist.gov/vuln/detail/CVE-2020-27663)|In GLPI before 9.5.3, ajax/getDropdownValue.php has an Insecure Direct Object Reference (IDOR) vulnerability that allows an attacker to read data from any itemType (e.g., Ticket, Users, etc.).|
|03/02/2021|[CVE-2021-21255](https://nvd.nist.gov/vuln/detail/CVE-2021-21255)|GLPI is an open-source asset and IT management software package that provides ITIL Service Desk features, licenses tracking and software auditing. In GLPI version 9.5.3, it was possible to switch entities with IDOR from a logged in user. This is fixed in version 9.5.4.|
|03/08/2021|[CVE-2021-21324](https://nvd.nist.gov/vuln/detail/CVE-2021-21324)|GLPI is an open-source asset and IT management software package that provides ITIL Service Desk features, licenses tracking and software auditing. In GLPI before version 9.5.4 there is an Insecure Direct Object Reference (IDOR) on "Solutions". This vulnerability gives an unauthorized user the ability to enumerate GLPI items names (including users logins) using the knowbase search form (requires authentication). To Reproduce: Perform a valid authentication at your GLPI instance, Browse the ticket list and select any open ticket, click on Solution form, then Search a solution form that will redirect you to the endpoint /"glpi/front/knowbaseitem.php?item_itemtype=Ticket&item_items_id=18&forcetab=Knowbase$1", and the item_itemtype=Ticket parameter present in the previous URL will point to the PHP alias of glpi_tickets table, so just replace it with "Users" to point to glpi_users table instead; in the same way, item_items_id=18 will point to the related column id, so changing it too you should be able to enumerate all the content which has an alias. Since such id(s) are obviously incremental, a malicious party could exploit the vulnerability simply by guessing-based attempts.GLPI is an open-source asset and IT management software package that provides ITIL Service Desk features, licenses tracking and software auditing. In GLPI before version 9.5.4 there is an Insecure Direct Object Reference (IDOR) on "Solutions". This vulnerability gives an unauthorized user the ability to enumerate GLPI items names (including users logins) using the knowbase search form (requires authentication). To Reproduce: Perform a valid authentication at your GLPI instance, Browse the ticket list and select any open ticket, click on Solution form, then Search a solution form that will redirect you to the endpoint /"glpi/front/knowbaseitem.php?item_itemtype=Ticket&item_items_id=18&forcetab=Knowbase$1", and the item_itemtype=Ticket parameter present in the previous URL will point to the PHP alias of glpi_tickets table, so just replace it with "Users" to point to glpi_users table instead; in the same way, item_items_id=18 will point to the related column id, so changing it too you should be able to enumerate all the content which has an alias. Since such id(s) are obviously incremental, a malicious party could exploit the vulnerability simply by guessing-based attempts.|
|03/08/2021|[CVE-2021-21326](https://nvd.nist.gov/vuln/detail/CVE-2021-21326)|GLPI is an open-source asset and IT management software package that provides ITIL Service Desk features, licenses tracking and software auditing. In GLPI before version 9.5.4 it is possible to create tickets for another user with self-service interface without delegatee systems enabled. This is fixed in version 9.5.4.|
|04/13/2021|[CVE-2021-29436](https://nvd.nist.gov/vuln/detail/CVE-2021-29436)|Anuko Time Tracker is an open source, web-based time tracking application written in PHP. In Time Tracker before version 1.19.27.5431 a Cross site request forgery (CSRF) vulnerability existed. The nature of CSRF is that a logged on user may be tricked by social engineering to click on an attacker-provided form that executes an unintended action such as changing user password. The vulnerability is fixed in Time Tracker version 1.19.27.5431. Upgrade is recommended. If upgrade is not practical, introduce ttMitigateCSRF() function in /WEB-INF/lib/common.php.lib using the latest available code and call it from ttAccessAllowed().|
|10/13/2021|[CVE-2021-41139](https://nvd.nist.gov/vuln/detail/CVE-2021-41139)|Anuko Time Tracker is an open source, web-based time tracking application written in PHP. When a logged on user selects a date in Time Tracker, it is being passed on via the date parameter in URI. Because of not checking this parameter for sanity in versions prior to 1.19.30.5600, it was possible to craft the URI with malicious JavaScript, use social engineering to convince logged on user to click on such link, and have the attacker-supplied JavaScript to be executed in user's browser. This issue is patched in version 1.19.30.5600. As a workaround, one may introduce `ttValidDbDateFormatDate` function as in the latest version and add a call to it within the access checks block in time.php.|
|10/18/2021|[CVE-2021-41156](https://nvd.nist.gov/vuln/detail/CVE-2021-41156)|anuko/timetracker is an, open source time tracking system. In affected versions Time Tracker uses browser_today hidden control on a few pages to collect the today's date from user browsers. Because of not checking this parameter for sanity in versions prior to 1.19.30.5601, it was possible to craft an html form with malicious JavaScript, use social engineering to convince logged on users to execute a POST from such form, and have the attacker-supplied JavaScript to be executed in user's browser. This has been patched in version 1.19.30.5600. Upgrade is recommended. If it is not practical, introduce ttValidDbDateFormatDate function as in the latest version and add a call to it within the access checks block.|
|12/21/2021|[CVE-2021-43851](https://nvd.nist.gov/vuln/detail/CVE-2021-43851)|Anuko Time Tracker is an open source, web-based time tracking application written in PHP. SQL injection vulnerability exist in multiple files in Time Tracker version 1.19.33.5606 and prior due to not properly checking of the "group" and "status" parameters in POST requests. Group parameter is posted along when navigating between organizational subgroups (groups.php file). Status parameter is used in multiple files to change a status of an entity such as making a project, task, or user inactive. This issue has been patched in version 1.19.33.5607. An upgrade is highly recommended. If an upgrade is not practical, introduce ttValidStatus function as in the latest version and start using it user input check blocks wherever status field is used. For groups.php fix, introduce ttValidInteger function as in the latest version and use it in the access check block in the file.|
|02/24/2022|[CVE-2022-24707](https://nvd.nist.gov/vuln/detail/CVE-2022-24707)|Anuko Time Tracker is an open source, web-based time tracking application written in PHP. UNION SQL injection and time-based blind injection vulnerabilities existed in Time Tracker Puncher plugin in versions of anuko timetracker prior to 1.20.0.5642. This was happening because the Puncher plugin was reusing code from other places and was relying on an unsanitized date parameter in POST requests. Because the parameter was not checked, it was possible to craft POST requests with malicious SQL for Time Tracker database. This issue has been resolved in in version 1.20.0.5642. Users unable to upgrade are advised to add their own checks to input.|
|02/24/2022|[CVE-2022-24708](https://nvd.nist.gov/vuln/detail/CVE-2022-24708)|Anuko Time Tracker is an open source, web-based time tracking application written in PHP. ttUser.class.php in Time Tracker versions prior to 1.20.0.5646 was not escaping primary group name for display. Because of that, it was possible for a logged in user to modify primary group name with elements of JavaScript. Such script could then be executed in user browser on subsequent requests on pages where primary group name was displayed. This is vulnerability has been fixed in version 1.20.0.5646. Users who are unable to upgrade may modify ttUser.class.php to use an additional call to htmlspecialchars when printing group name.|
