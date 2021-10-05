## The HTTP Request Lifecycle


![image](https://csharpcorner-mindcrackerinc.netdna-ssl.com/article/introduction-to-iis-server-http-request-life-cycle-hosting-a-website-in-iis-se/Images/image005.png)

### Local Processing
- Your browser extracts the "scheme"/protocol (we have established
that this will be HTTP).
- The browser has the intended hostname for the request, it needs to resolve an IP address.

### Resolve an IP
- Like the processing done locally, resolving an IP from a "DNS server" is a sequence that includes many steps, and includes failovers if the first request fails to return an address.
- The DNS request contains the preconfigured IP for your DNS server and your return IP in its header. The hostname for which you are trying to resolve an IP is in the request’s "Question" section.
- Your request will now have to travel many network devices to reach its target DNS server.
- Once your request arrives at your configured DNS server, the server looks for the address associated with the requested hostname. If it finds one, it sends a response.
- If the response makes it back, the requesting client now has a target IP.

### Establish a TCP Connection
- Now that the client has an IP address, it can send an HTTP request, right? Almost, but first, since the request is sent over TCP, which is a transport layer protocol like UDP, the client must open a TCP connection.

### Send an HTTP Request
- now that the client has an IP address and a TCP connection, it can finally send an HTTP request.
- The request is made up of a "request line", request header, and a body. The "request line" is simply a line that indicates the HTTP method, the resource being requested, and the protocol version.

### Tearing Down and Cleaning Up
- Once the response has been fully delivered, the client sends a FIN packet at the TCP level, to which the server responds with an ACK, and then generally sends a FIN of its own, which the client responds to with its own ACK signal.
- your browser begins processing what it has received.

## How to Do a Simple HTTP Request in Java
- HttpUrlConnection
- Creating a Request
- Adding Request Parameters
- Setting Request Headers
- Configuring Timeouts
- Handling Cookies
- Handling Redirects
- Reading the Response
- Reading the Response on Failed Requests
- Building the Full Response
