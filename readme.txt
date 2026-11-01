A lightweight Python script that performs an HTTP HEAD request on a target URL to quickly gather basic server information,
HTTP status codes, technologies, and cookies.

features: easily identifies standard response states.
          Detects the underlying server software(Server Header).
          Checks for backend technologies via the X-Powered-By header.
          Displays cookies and specifically checks for session identifiers.

Make sure you have Python installed along with the requests library. You can install the required dependency using pip 
  "pip install requests"

Usage:
      1. run the script [python scanner.py]
      2. Enter the target URL when prompted [https://example.com]

Output: 
      [Input]:https://example.com
      [DOMAIN]  https://example.com
      [STATUS]: OK
      [COOKIES] <RequestsCookieJar[]>
      [SERVER]  ECS (sec/9745)
      [BACKEND] Not found
The script utilizes the requests.head() method, which fetches only the headers of a web page rather than the full body content, making it fast and efficient for reconnaissance and banner checking.

        

