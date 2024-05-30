## IP Address: Your Device's Unique ID

Imagine a big city with lots of houses. Each house needs a unique address so the mail carrier can find it, right? <br />
An IP address is like a house address for your devices on the internet. It lets other devices know exactly where to send information.<br />

IPv4: This is the most common type of IP address. It uses a system of four numbers separated by dots (like 192.168.1.100). Each number can be between 0 and 255.<br />
Why are IP Addresses Important?<br />
Finding Devices: Just like you need an address to find a house, other devices on the internet need an IP address to find your computer, phone, or tablet.<br />
Sending Information: When you browse the web, your computer uses your IP address to tell websites where to send the information you request.<br />
Security: IP addresses can be used to control who can access your network or certain websites.<br />

most of the times when we talk about private subnets you will see this numbers only 192.0.0.0 or 172.0.0.0 or 10.0.0.0  because these are the ones that are used for private subnets just like a standard practice as others are used for public ips

## Subnet: Dividing Your Network <br />

example - finance ke liye alag subnet bna do for security purpose <br />

Subnets are like dividing your network into smaller, more manageable groups for different purposes.<br />

Why Use Subnets?<br />
Security: Subnets help keep your devices safe by isolating them into different groups. If one device gets infected with a virus, it's less likely to spread to other devices on a different subnet.<br />
Organization: Subnets make it easier to manage your network by dividing it into logical groups. You can have a subnet for your computers, another for your printers, and another for your smart home devices.<br />

there are two types of subnets one is private subnet two is public subnet if you ever used the cloud provider you might have uh heard about this terms called private and public subnet but what exactly are these so private subnet is some Network that does not have access to Internet and public subnet is a subnet that has access to Internet that's the only difference. how do you do that how can you enable access to Internet don't worry it's a very simple concept uh you know if you already know about Cloud providers like AWS or Azure all that you need to do is you can go to this particular subnets and you can attach route tables to this particular subnet and destination of a particular route of this subnet you can provide as an internet gateway and that will grant access to the internet.

## CIDR:<br />

to describe How Many Devices Can Join.<br />

CIDR (Classless Inter-Domain Routing) is a way to describe how many IP addresses are available/allocated within a subnet. It's like saying "this subnet has room for 256 devices" or "this subnet has room for 1024 devices."<br />

CIDR Notation: CIDR uses a slash (/) followed by a number to indicate the size of the subnet. For example:<br />
192.168.1.0/24: This subnet has 256 IP addresses available.<br />
10.0.0.0/16: This subnet has 65,536 IP addresses available.<br />
How to Calculate CIDR:<br />

Start with 32: An IPv4 address has 32 bits.<br />
Subtract the CIDR number: For example, in 192.168.1.0/24, subtract 24 from 32, which equals 8.<br />
Calculate 2 to the power of the result: 2 to the power of 8 is 256. This means there are 256 IP addresses available in the subnet.<br />
Example: Setting up a Subnet<br />

Let's say you're setting up a network for your small business. You want to have a subnet for your employees' computers and another subnet for your printers.<br />

Choose an IP Address Range: You might choose the range 192.168.1.0 to 192.168.1.255 for your network.<br />
Create the Subnets:<br />
Employee Computers: You could use the CIDR notation 192.168.1.0/24 for your employee subnet. This would give you 256 IP addresses for your employees.<br />
Printers: You could use the CIDR notation 192.168.1.128/25 for your printer subnet. This would give you 128 IP addresses for your printers.<br />
Key Takeaways<br />

IP addresses: Unique identifiers for devices on a network.<br />
Subnets: Divide a network into smaller, more manageable groups.<br />
CIDR: Describes how many IP addresses are available within a subnet.<br />

![Learn Networking in 3 Hours _ Networking Fundamentals + AWS VPC Networking 13-12 screenshot](https://github.com/HimanshuMishra123/Networking/assets/164254902/55450f83-0e42-4953-8ec9-78c56168bda0)

![Learn Networking in 3 Hours _ Networking Fundamentals + AWS VPC Networking 23-10 screenshot](https://github.com/HimanshuMishra123/Networking/assets/164254902/655f6783-e7ef-44c1-ad85-376f643f937c)

![Learn Networking in 3 Hours _ Networking Fundamentals + AWS VPC Networking 27-19 screenshot](https://github.com/HimanshuMishra123/Networking/assets/164254902/3d37f243-14cc-4440-a0b6-0114b0978a8b)


