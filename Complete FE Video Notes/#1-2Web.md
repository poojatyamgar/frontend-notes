---
marp: true
---

# Video 1 - has link to drive containing materials

# Video 2 has following details

# Why do we need web app(Real time examples of growing online business and services.)

 ## Why learn to create Web Applications

 + Websites and Web Applications help businesses.
   Offline to Online or Fully Online.

 + Evolving business challenges require technology solutions as
   business grows.

  + Custom web application development solutions can automate business
    processes and provide a superior ROI to investments.
    
  + Eg:- 1mg, healthifyme, Social Media, ecommerce, Delivery Services,
         Financial online services, Entertainment sites, Travel booking websites,
         Communication services.
---

+ How does the internet work ?
	+ It is line with many computers connected to each other.
	+ Some are online for 24*7-->Web Servers.
	+ Servers are like libraries open all day for us to request any book
        (websites) and read any of its page(webpage).

                                                                Server
------------------------------------------------------------------|----
         |
        Computer(Client)------Internet Service Provider------DNS Server
                               (Internet)
       + So, Internet is basically a backbone of sending and receiving requests
          and responses.

---

+ Basic Network Ideas :-
   	
       + So for the entire(internet) process of sending and receiving responses we have a 
          we have a 4 layer protocol/service of web application.
	 
          + I) Application (DNS, HTTP)

            + The protocols used in application layer is "HTTP"
            + "https://www.facebook.com/"
              scheme://prefix.domain:port/path/filename
              Type of internet service,https->secured protocol for money transactions and etc is used.
              Domain prefix
              Internet domain name
              Port number at the host (fefault for http is 80)
              Path at the server (If omitted: the root directory of the site)
              filename, the name of a document or resource.
            + As internet is a backbone, in real there are a number of huge optical fibres    
              connection between the cities and 
              countries across the world, these are used to have internet communication, which is going to cater a very fast internet request.  
              (Eg:- Our requests our send to server and we recive responses within milliseconds.)
            + The internet backbone is connected to various networks(LAN, WAN), all these networks 
                are interconnected to each other and at the gateway of every network is a modem.
                Each network consists of a number of computers (Clients, Servers)
                Each device(computer) as a specific IP address 32 bit divided into 4 parts each of 8 bits.
                (0.0.0.0) to and in between (225.225.225.225), eg:(129.51.150.10)
              + The above mentioned device with IP address want to access the google browser
                The Ist thing would finding for (google.com) within the network.
                Since the server is not present within the network. So the request goes out of the network
                towards the address which it seraches for, so the Ist thing it comes is the modem, firewall(software, determines whether the request is a safe or unsafe, if the request is unsafe it blocks it then and there.),
                ISP(Internet Service Provider)-->DNS(Domain Name Server) 

---

        + II) Transport (TCP[Transmission Control Protocol]

		      This layer helps us in communicating without corrupting or loosing data.
          This layer uses a TCP Protocol, TCP defines how applications can create reliable channels of communications across the network.
          So, once we have communicated our data without corrupting or loosing it over a reliable 
          channel taken care of by TCP, we are rest assured that our application which is run in the client or the other application which is run on server 
          is able to communicate. 

---

        + III) Network (IP [Internet Protocol])

		      This layer is concerned with address and routing. It will understand the ours,and client address and it will know which is the server address which we are sending the request for.
          This layer uses a protocol called (IP),
					The IP defines how computers can get data to each other over routed interconnected set of networks.
          Internet has a lot of interconnected networks which are connected to each other
          How does the data go from one address to the other is taken care of network layer.
            
---

        + IV) Network Interface (Ethernet)

		      Our (Device)Laptop is connected over the internet using ethernet connection.This ethernet,
		      is the protocol or service of our network interface. This network interface is 
          actually a physical interface which is connecting us to the internet.
          Now, as we send request, it basically goes to the "network layer".

---     

#  The Browser and HTTP

+ Data is sent and received in packets in TCP/IP
+ Packet :   Data (SOURCE : 129.51.150.10
                   DESTINATION : 64.233.171.1)
+ Web operates on top of the internet via HTTP (Hyper Text Transfer Protocol)
+ www is a system of interlinked webpages accessed via the internet.
+ HTTP is a stateless protocol
+ Browser is a piece of software that allows to lookup IP address,
  to send and receive data.

---

# What are websites and how do they work

+ Any book in the library of www with all of its pages(webpages)
  is a website

---

# How web applications evolved

# Web application architecture

+ Front End        →    MiddleWare         →  HTTP request → DataBase ([MYSQL, Postgre SQL,]
  (HTML, CSS, JS,       (JAVA, PYTHON,C,   ←  HTTP response ← DataBase  [Mongodb, Cassandra, Oracle])
  REACT, ANGULAR,        PHP, NODEJS)
  BOOTSTRAP)  
                            

                   ←      ↑  API Service Providers  ↑    →

---

