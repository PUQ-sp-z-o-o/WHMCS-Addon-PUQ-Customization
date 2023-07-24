# Forward/Reverse DNS Zones for IPv4 and IPv6

##### **Configuring Forward and Reverse DNS Zones for IPv4 and IPv6**

DNS zones are used to translate domain names into IP addresses and vice versa. To properly configure forward and reverse DNS zones for IPv4 and IPv6, you need to know the subnets associated with the respective IP addresses. Below are instructions on how to build zones for IPv4 and IPv6.

##### **Forward DNS Zones for IPv4/IPv6:**

Forward DNS zones are used to map domain names to IPv4 addresses.

1. Determine the domain name for your server or device. For example: myserver.example.com.
2. Determine the IPv4 address that will correspond to this domain name. For example: 203.0.113.10.

<div id="bkmrk-myserver.example.com"><div>`myserver<span class="hljs-selector-class">.example</span><span class="hljs-selector-class">.com</span>.       IN      <span class="hljs-selector-tag">A</span>       <span class="hljs-number">203.0</span>.<span class="hljs-number">113.10</span>`</div></div><div id="bkmrk-"></div><div id="bkmrk-determine-the-ipv6-a">1. Determine the IPv6 address that will correspond to this domain name. For example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334.

</div><div id="bkmrk-myserver.example.com-0"><div>`<span class="hljs-string">myserver.example.com.</span>       <span class="hljs-string">IN</span>      <span class="hljs-string">AAAA</span>    <span class="hljs-number">2001</span><span class="hljs-string">:0db8:85a3:0000:0000:8a2e:0370:7334</span>`</div><div></div></div>##### **Reverse DNS Zones for IPv4 and IPv6:**

Reverse DNS zones convert IP addresses back into domain names. Please note that reverse DNS zones for IPv4 and IPv6 have slightly different formats.

##### **Reverse DNS Zones for IPv4:**

Reverse DNS zones for IPv4 are based on the four octets of an IPv4 address.

1. Split the IPv4 address into octets and reverse them, adding ".in-addr.arpa" at the end.   
    For example: **10.113.0.203.in-addr.arpa**
2. Create a new zone in the DNS configuration file (e.g., reverse.db) with the specified reverse domain name and your server's domain name:

<div id="bkmrk-10.113.0.203.in-addr"><div></div><div>`10.113.0.203.in-addr.arpa.  IN      PTR     myserver.example.com.`</div></div>##### **Reverse DNS Zones for IPv6:**

Reverse DNS zones for IPv6 are based on the hexadecimal representation of the IPv6 address.

1. Write the IPv6 address in hexadecimal form, separating each group of digits with colons and adding ".ip6.arpa" at the end.   
    For example: **4.3.3.7.0.e.3.7.0.2.e.a.8.0.0.0.0.0.0.0.0.0.0.0.3.8.a.5.8.b.d.0.1.0.0.2.ip6.arpa**
2. Create a new zone in the DNS configuration file (e.g., reverse.db) with the specified reverse domain name and your server's domain name:

<div id="bkmrk-4.3.3.7.0.e.3.7.0.2."><div></div><div>`4.3.3.7.0.e.3.7.0.2.e.a.8.0.0.0.0.0.0.0.0.0.0.0.3.8.a.5.8.b.d.0.1.0.0.2.ip6.arpa.  IN      PTR     myserver.example.com.`</div></div><div id="bkmrk--0"><div></div></div><div id="bkmrk--1"><div></div></div>