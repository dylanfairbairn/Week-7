# Week-7

Pentesting Report
XSS Script Error alert
Summary: Creating a user account in WordPress. 
Vulnerability types: XSS
Tested in version: 4.1
Fixed in version: 4.1.19
GIF Walkthrough: source: LICEcap 
Steps to recreate: Login to the user that you created. Go to the site and post a comment on the website with the Xss script. The xss script I used was IMG SRC="#" ONERROR="alert('Hacked')". So anytime the page loads an error pops up with "Hacked".
XSS Script onmouseover error
Summary: Showing a xss scripting error for when your mouse goes over a link or something in the site.
Vulnerability types: XSS onmouseover error
Tested in version: 4.1
Fixed in version: 4.1.19
GIF Walkthrough: source: LICEcap
Steps to recreate: Log into the user you created. Go to the wpdistillery site, post a comment and use the xss script <b onmouseover=alert('Hacked!')>click me!. When the admin user logs in and sees this, when he roles the mouse over the "click me!" it'll pop up an error "Hacked".
WPScan Dictionary attack
Summary: Using wordpress to dictionary attack a WordPress site.
Vulnerability types: Dictionary attack
Tested in version: 4.1
Fixed in version: 4.1
GIF Walkthrough: source: LICEcap
Steps to recreate: Run wpscan --url http://wpdistillery.vm/wp-login.php? --wordlist passwords --username admin. Make sure your wordlist is the wordlist you created.
