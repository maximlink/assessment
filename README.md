# Assessment App

**ONLY AVAILABLE AS CUSTOM APP VIA APPLE SCHOOL/BUSINESS MANAGER**

--Simple iPadOS app to enable live proctoring of web-based assessment exams--

Assessment displays camera view and web-based exam in a single app. The app is intended to be used in conjunction with third video sharing solutions such as Zoom. Exam taker can share iPad screen with Assessment running in foreground (live camera and exam displayed) while sharing screen with the exam proctor.

Assessment app leverages the power of Jamf and managed app configuration. Configurable features include screenshot detection, camera enablement, custom UI and exam view size.

Assessment requires managed distribution and is only available as a Custom App via Apple School Manager or Apple Business Manager.

Please e-mail assessment@maximlink.com to request access.  Include your ASM/ABM Organization Name and ID with the request.

# Managed App Config

URL - URL of LMS / Assessment Site

SCREEN RATIO - percentage of screen dedicated to web site

CAMERA_TOGGLE_ENABLE (NO/YES) - enable user to be able to turn off camera

CAMERA_LETTERBOX_COLOR (hex color) - color of space above and below camera preview

SCREEN_HEADER_TITLE - label in top center when browser bar is not enabled

SCREEN_HEADER_MAIN_COLOR (hex color) - color of header background

SCREEN_HEADER_SECONDARY_COLOR (hex color) - color of icons in header

BROWSER_BAR_ENABLE (YES/NO) - enable user to enter URL and navigate

SCREEN_CAPTURE_MODE (1/2/3) - 1: no effect; 2: warns if screenshot taken; 3: locks app if screenshot taken and force quit required

# AppConfig Template

```
<dict>
 <key>URL</key>
    <string>https:/your_exam_site.edu/</string>
 <key>SCREEN_RATIO</key>
    <string>75</string>
 <key>CAMERA_TOGGLE_ENABLE</key>
    <string>NO</string>
 <key>CAMERA_LETTERBOX_COLOR</key>
    <string>#000000</string>
 <key>SCREEN_HEADER_TITLE</key>
    <string>Powered by Jamf</string>
 <key>SCREEN_HEADER_MAIN_COLOR</key>
    <string>#00274C</string>
 <key>SCREEN_HEADER_SECONDARY_COLOR</key>
    <string>#FFFFFF</string>
 <key>BROWSER_BAR_ENABLE</key>
    <string>NO</string>
 <key>SCREEN_CAPTURE_MODE</key>
    <string>1</string>
</dict>
```


