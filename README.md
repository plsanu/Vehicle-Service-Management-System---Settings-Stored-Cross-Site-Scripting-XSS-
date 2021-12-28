# Vehicle Service Management System - 'Settings' Stored Cross Site Scripting (XSS)
Vehicle Service Management System - 'Settings' Stored Cross Site Scripting (XSS)

### Exploit Title: Vehicle Service Management System - 'Settings' Stored Cross Site Scripting (XSS)
### Date: 29/12/2021
### Exploit Author: P.L.Sanu
### Exploit Author Website: https://www.plsanu.com
### Vendor Homepage: https://www.sourcecodester.com
### Software Link: https://www.sourcecodester.com/php/14972/vehicle-service-management-system-php-free-source-code.html
### Version: <= 1.0
### Tested on: Windows 10
### CVE : 
### Google Dork: N/A
### Reference: 
- https://www.plsanu.com/vehicle-service-management-system-settings-stored-cross-site-scripting-xss
- https://github.com/plsanu/Vehicle-Service-Management-System-Settings-Stored-Cross-Site-Scripting-XSS

### Steps to Reproduce:
1. Login to the admin panel http://localhost/vehicle_service/admin
2. Navigate to Settings section http://localhost/vehicle_service/admin/?page=system_info
3. Inject the payload "><script>alert(document.cookie)</script> in System Name, System Short Name & About Us input field.
4. Click on update button.
5. Malicious javascript code triggered.
