---
marp: true
paginate: true
footer: '![width:200px](./images/header_logo.png)'
---
## How WebSite works
1. You type www.skill-lync.com into the address bar of your browser.
2. The browser checks the cache for a DNS record to find the corresponding IP address of www.skill-lync.com (This is called as DNS looking)
    + browser cache
    + os cache
    + router cache
    + ISP cache

 > A cache is a special storage space for temporary files that makes a device, browser, or app run faster and more efficiently.

---
3. If the requested URL is not in the cache, ISP’s DNS server initiates a DNS query to find the IP address of the server that hosts www.skill-lync.com

4. The browser initiates a TCP connection with the server.
    > This connection is established using a process called the TCP/IP three-way handshake. This is a three-step process where the client and the server exchange SYN(synchronize) and ACK(acknowledge) messages to establish a connection.

---
### Three way handshake
1. The client machine sends a SYN packet to the server over the internet, asking if it is open for new connections.

2. If the server has open ports that can accept and initiate new connections, it’ll respond with an ACKnowledgment of the SYN packet using a SYN/ACK packet.

3. The client will receive the SYN/ACK packet from the server and will acknowledge it by sending an ACK packet.

Then a TCP connection is established for data transmission!

---
5. The browser sends an HTTP request to the webserver.

6. The server handles the request and sends back a response (This is responsibility of Backend, what to return, and in what format)

7. The server sends out an HTTP response
    ```
    Request URL: https://skill-lync.com/
    Request Method: GET
    Status Code: 200 
    Remote Address: 104.26.2.172:443
    Referrer Policy: strict-origin-when-cross-origin
    age: 57800
    cache-control: s-maxage=31536000, stale-while-revalidate
    cf-cache-status: DYNAMIC
    cf-ray: 71c2ab630f871be7-DEL
    content-encoding: br
    content-type: text/html; charset=utf-8
    date: Thu, 16 Jun 2022 09:55:22 GMT
    ```

---
8. The browser displays the HTML content

    >The browser displays the HTML content in phases. First, it will render the bare bone HTML skeleton. Then it will check the HTML tags and send out GET requests for additional elements on the web page, such as images, CSS stylesheets, JavaScript files, etc. These static files are cached by the browser, so it doesn’t have to fetch them again the next time you visit the page. In the end, you’ll see www.skill-lync.com appearing on your browser.
