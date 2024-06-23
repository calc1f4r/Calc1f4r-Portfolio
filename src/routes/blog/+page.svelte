<script>
	let blogs = [
		{
			title: 'Uploading files to Arweave using arweave.js',
			description:
				'In this article, we will learn how to confidently upload files onto Arweave using its SDK library Arweave.js.',
			image: 'https://miro.medium.com/v2/resize:fit:1400/format:webp/1*LzFK-fOVUP2LJBM87y91Eg.png',
			link: 'https://medium.com/@calc1f4r/uploading-files-to-arweave-using-arweave-js-1102f8da5663'
		},
		{
			title: 'The Ultimate Guide to Port Scanning using Nmap | Nmap Notes ',
			description:
				'Nmap is a powerful tool for network discovery and security auditing. It’s used by hackers, system administrators, and cybersecurity professionals to scan networks, identify open ports, and detect vulnerabilities. In this blog post, we’ll cover the basics of Nmap, including installation, scanning techniques, and common use cases. Whether you’re a beginner or an experienced hacker, this guide will help you master Nmap and take your hacking skills to the next level.',
			image: 'https://hacklido.com/assets/files/2023-06-01/1685628833-697225-nmap.jpg',
			link: 'https://hacklido.com/blog/464-the-ultimate-guide-to-port-scanning-using-nmap-nmap-notes'
		},
		{
			title: 'Linux for hackers - Part #1 | Introduction to Linux and basics for hackers',
			description:
				'Whether you’re a beginner or an experienced hacker, this series will equip you with the knowledge to leverage Linux for hacking adventures. Linux’s flexibility, security, and vast array of tools make it an ideal platform for ethical hacking. In this first blog post, we’ll cover the basics, including command-line skills, file systems, permissions, and the importance of networking and security.',
			link: 'https://hacklido.com/blog/447-linux-for-hackers-part-1-introduction-to-linux-and-basics-for-hackers',
			image:
				'https://hacklido.com/assets/files/2023-05-25/1684997746-247329-linux-for-hackers-1.png'
		},
		{
			title: 'Linux for hackers - Part #2 | Linux Process and Storage Management',
			description:
				'Just like the other blog In this blog, we will go dive into topics like Linux processes and its management and In this blog we will also learn the storage/ partition management in Linux.',
			link: 'https://hacklido.com/blog/474-linux-for-hackers-part-2-linux-process-and-storage-management',
			image: 'https://hacklido.com/assets/files/2023-06-04/1685902129-713451-linux-for-hackers.png'
		},
		{
			title:
				'Linux for hackers - Part #3 | Logical Volume Management and Managing Basic Hardware devices',
			description:
				'LVM is a flexible storage management system that lets us handle disk space dynamically. It’s a must-know tool for hackers and system administrators. We’ll cover everything from creating and resizing logical volumes to working with snapshots and mirroring. In addition, understanding how to manage hardware in Linux is crucial for effective hacking. We’ll dive into device files, module management, and optimizing hardware components for peak performance.',
			link: 'https://hacklido.com/blog/482-linux-for-hackers-part-3-logical-volume-management-and-managing-basic-hardware-devices',
			image: 'https://hacklido.com/assets/files/2023-06-08/1686204789-140049-linux-for.png'
		},
		{
			title: 'Linux for hackers - Part #4 | Network Scanning and Enumeration with Linux',
			description:
				'Linux is a powerful platform for hacking, and understanding networking and security is essential for any hacker. In this blog post, we’ll cover the basics of networking, including IP addresses, routing, and firewalls. We’ll also explore security concepts such as encryption, authentication, and intrusion detection. By the end of this series, you’ll have the knowledge and skills to leverage Linux for hacking adventures.',
			link: 'https://hacklido.com/blog/486-linux-for-hackers-part-4-network-scanning-and-enumeration-with-linux',
			image: 'https://hacklido.com/assets/files/2023-06-13/1686618507-371406-image.png'
		},
		{
			title: 'Linux for hackers - Part #6 | Digital Forensics with Linux',
			description:
				'Digital forensics, also known as computer forensics or cyber forensics, is the branch of forensic science that deals with the identification, preservation, collection, analysis, and presentation of digital evidence in legal and investigative contexts.',
			link: 'https://hacklido.com/blog/490-linux-for-hackers-part-5-digital-forensics-with-linux',
			image: 'https://hacklido.com/assets/files/2023-06-14/1686762045-656490-linux-for-3.png'
		},
		{
			title: 'Burpsuite 101: Introduction and Installation',
			description:
				'The focus of this series is on Burp Suite’s potential as the ultimate tool for security enthusiasts and hackers. 🛡️ The purpose of “Burp Suite for Hackers 101” is to give you the information and abilities necessary to use Burp Suite to the fullest extent possible. This series will have something for everyone, regardless of your level of experience or desire to improve. 📈',
			link: 'https://hacklido.com/blog/621-burpsuite-101-introduction-and-installation',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1697189974079/edabe5bd-6638-474b-8311-15a58231d782.png'
		},

		{
			title: 'Burp Suite 101: Exploring Burp Proxy and Target Specification ',
			description:
				'Hello there, readers. Welcome back to the third chapter of the blog series “Burpsuite 101,” “Exploring burp proxy and target scoping.” This blog dives further into the capabilities of Burp Suite, concentrating on the core components of Burp Proxy and the art of accurate target scoping. Prepare to discover critical ideas that can help you improve your web application security testing game. Let’s get started! 🕵️‍♂️💻🌐',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1697307344546/8e15b4ac-10a5-4e86-bb1a-9751279dde99.png',
			link: 'https://hacklido.com/blog/625-burp-suite-101-exploring-burp-proxy-and-target-specification'
		},
		{
			title: 'Burpsuite 101: Exploring Burp Repeater and Burp Comparer',
			description:
				'Hello and welcome back to the fourth part of our “Burpsuite 101” series, where we keep things easy and effective. Today, we’re going to explore “Burp Repeater and Burp Comparer.” 🚀 These useful web testing tools will assist you in improving your HTTP requests and analyzing results. Ready to learn the secrets of Burp Repeater and Burp Comparer and level up your online security game? Let’s get started! 🕵️‍♂️💻🔍',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1697359842360/44820d09-1b35-4017-90e8-e35027fd4a93.png',
			link: 'https://hacklido.com/blog/628-burpsuite-101-exploring-burp-repeater-and-burp-comparer'
		},
		{
			title: 'Burpsuite 101 : Going deep Into intruder',
			description:
				'Burp Intruder is the answer to fully automating web application testing, discovering vulnerabilities, and analyzing online applications. Whether you’re new to web security or an expert in the field, this article will provide you with the knowledge and skills you need to explore all of Burp Intruder’s features.',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1698672013364/10b3bd93-9c7e-4373-b6fb-cd608108583b.png',
			link: 'https://hacklido.com/blog/631-burpsuite-101-going-deep-into-intruder'
		},
		{
			title: "Beginner's Guide to Wireless Hacking #1 | From Signals to Secrets ",
			description:
				'Wi-Fi is everywhere these days, connecting our devices and allowing us to access information and communicate effortlessly. But have you ever wondered how it actually works? And is it possible to manipulate Wi-Fi networks for different purposes? In this series “A Beginner’s Guide to Wireless Hacking”, we will go deep into the architecture and will learn what vulnerabilities can affect our Wifi and How can we exploit WiFi.',
			image: 'https://hacklido.com/assets/files/2023-06-19/1687203671-749444-linux-for-12.png',
			link: 'https://hacklido.com/blog/494-beginners-guide-to-wireless-hacking-1-from-signals-to-secrets'
		},
		{
			title: "A Beginner's Guide to Wireless Hacking #2 | Spoofing ",
			description:
				'Spoofing means pretending to be something or someone you’re not. It’s like wearing a disguise to trick others. It involves creating a fraudulent representation of something or someone to gain unauthorized access, mislead individuals, or compromise the integrity of systems or communications.',
			image: 'https://hacklido.com/assets/files/2023-06-21/1687324017-754669-wireless-hacking.png',
			link: 'https://hacklido.com/blog/502-a-beginners-guide-to-wireless-hacking-2-spoofing'
		},
		{
			title: "A Beginner's Guide to Wireless Hacking #3| Hacking WEP Protocol",
			description:
				'It’s time for the third blog “Hacking WEP” of our blog series on “A Beginner’s Guide to Wireless Hacking.” In this blog we will explore the Wired Equivalent Privacy (WEP) protocol in a concise way. You’ll learn how WEP functions, find out how airplay-ng cracks WEP, and gain practical tips on how to hack WEP. So let’s start 😉!',
			image:
				'https://hacklido.com/assets/files/2023-06-25/1687679010-314100-linux-for-compressed.jpg',
			link: 'https://hacklido.com/blog/506-a-beginners-guide-to-wireless-hacking-3-hacking-wep-protocol'
		},
		{
			title: "A Beginner's Guide to Wireless Hacking #4 | Hacking WPA ",
			description:
				'Welcome to the fourth blog “Hacking WPA”of the series folks!⚡.In this blog, we’ll go deep into how WPA works, the encryption it offers, various methods used to hack WPA, and essential insights into protecting your own network.',
			image: 'https://hacklido.com/assets/files/2023-07-01/1688196743-678997-linux-for-10.png',
			link: 'https://hacklido.com/blog/520-a-beginners-guide-to-wireless-hacking-4-hacking-wpa'
		},
		{
			title: "Beginner's Guide to Wireless Hacking #5 | Exploring Evil Twin Attacks",
			description:
				'Welcome to the fifth blog “Hacking WPA”of the series folks!⚡. In this blog, we’ll go deep into Evil twin attacks , how they work , how can you perform them, and various safeguards to protect you against them.',
			image: 'https://hacklido.com/assets/files/2023-08-05/1691278984-111549-linux-for.png',
			link: 'https://hacklido.com/blog/582-beginners-guide-to-wireless-hacking-5-exploring-evil-twin-attacks'
		},
		{
			title: 'Python for Hackers #1 | SSH Bruteforcer using Asynchronous Programming ',
			description:
				'Python for Hackers is a Python security tool-making series, in which I will teach you how to make some of the tools that you use in your life while pen-testing and forensics. You may ask why Python, because coding in Python is hell easy AF.',
			link: 'https://hacklido.com/blog/525-python-for-hackers-1-ssh-bruteforcer-using-asynchronous-programming',
			image:
				'https://hacklido.com/assets/files/2023-07-04/1688453228-394850-your-wish-if-u-want-to-take-this-compressed.jpg'
		},
		{
			title: 'Python for Hackers #2 | FTP Bruteforcer using asynchronous Programming',
			description:
				'we will learn about FTP and how it can be attacked using brute force techniques. For those of you who don’t know Asynchronous programming or haven’t read my previous blog, don’t worry I will discuss the topic of Asynchronous Programming here as well.',
			link: 'https://hacklido.com/blog/526-python-for-hackers-2-ftp-bruteforcer-using-asynchronous-programming',
			image:
				'https://hacklido.com/assets/files/2023-07-10/1688991148-975495-your-wish-if-u-want-to-take-this-3-compressed.jpg'
		},
		{
			title: 'Python for Hackers #3 | Building Directory Buster using asynchronous programming ',
			description:
				'Welcome to the “Python for Hackers” blog series! In this edition, we’ll create a powerful tool called “Directory Buster” using Asynchronous Programming. It’ll help us find hidden web resources swiftly and efficiently. In this blog, I will explain most of the necessary details required to build this.',
			link: 'https://hacklido.com/blog/565-python-for-hackers-3-building-directory-buster-using-asynchronous-programming',
			image:
				'https://hacklido.com/assets/files/2023-08-05/1691227593-766237-your-wish-if-u-want-to-take-this-5-compressed.jpg'
		},
		{
			title: 'Python for hackers #4 | Building Arp Spoofing/Posioning Script ',
			description:
				'👋 Welcome to the fourth blog of our “Python for Hackers” series! 🐍 In this chapter, we’ll dive intoARP cache poisoning and create a powerful script using Python. 😎 Let’s understand ARP spoofing and learn to build the tool used for poisoning!',
			link: 'https://hacklido.com/blog/580-python-for-hackers-4-building-arp-spoofingposioning-script',
			image:
				'https://hacklido.com/assets/files/2023-08-06/1691324389-961355-your-wish-if-u-want-to-take-this-6-compressed.jpg'
		},
		{
			title: 'Python For Hacker #5 | Building A Mutlithreaded Network Scanner',
			description:
				'Hello, readers 🙌 Yes, I am truly sorry for not being more active on this “Python For Hackers” series for such a long period. However, I will now carry on with this series. In this “Python for Hackers” blog post, I’ll explain how to create a Network scanner in Python that will enable you to identify clients that are available in your subnet and determine which ports are open on those clients. ',
			link: 'https://hacklido.com/blog/642-python-for-hacker-5-building-a-mutlithreaded-network-scanner',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1698673241597/e323637b-3804-4e2b-8ed2-758b57d0160e.png'
		},
		{
			title: 'Python For Hackers #6 | Building A Recursive Web Crawler ',
			description:
				'Welcome to the sixth blog of our “Python for Hackers” blog series. Today, we’re building a very easy to make tool which is Recursive web crawler with Python , which will help us scrape a whole page and find various important things for a web page.',
			link: 'https://hacklido.com/blog/647-python-for-hackers-6-building-a-recursive-web-crawler',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1698841137688/bfa2c016-d580-4694-ab5b-b86ffabd6078.png'
		},
		{
			title: 'Python for Hackers #7 | Building a multithreaded Subdomain Bruteforcer',
			description:
				'Subdomain brute forcing is a method for discovering subdomains of a target domain. It operates by attempting to resolve a list of common subdomain names against the DNS servers of the target domain. If the DNS server delivers a valid IP address for a subdomain, that subdomain is deemed valid.',
			link: 'https://hacklido.com/blog/653-python-for-hackers-7-building-a-multithreaded-subdomain-bruteforcer',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1698862505870/4708f496-0351-4b1e-b181-01765824534c.png'
		},
		{
			title: 'Python For Hackers #8 | Building A PDF Password Brute Forcer',
			description:
				' Welcome to the eighth blog of our “Python for Hackers” blog series. Today, we’re building a very easy to make tool which is Password Protected PDF file Bruteforcer with Python , which will help us Bruteforce every password file using a rainbow table attack.',
			link: 'https://hacklido.com/blog/654-python-for-hackers-8-building-a-pdf-password-brute-forcer',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1699251393104/6c100b9c-ed0f-46f7-b812-0818433955cf.png'
		},
		{
			title: 'Python For Hackers #9 | Building a Hash Cracker ',
			description:
				' In this blog of the series “Python For Hackers”, we are again building an easy tool which is a hash cracker, which helps us to crack the hash and get its original value.',
			link: 'https://hacklido.com/blog/655-python-for-hackers-9-building-a-hash-cracker',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1699282954297/9b3ecf37-b8cd-46ec-94e4-44e02359b691.png'
		},
		{
			title: 'Python For hackers #10 | Building a reverse shell ',
			description:
				'A reverse shell is a kind of remote shell that enables an attacker to connect to a remote system and execute commands as if they were physically present at the victim’s computer. In a reverse shell attack, the victim’s system connects to the attacker’s system rather than the attacker connecting to the victim’s system. ',
			link: 'https://hacklido.com/blog/656-python-for-hackers-10-building-a-reverse-shell',
			image:
				'https://cdn.hashnode.com/res/hashnode/image/upload/v1699289410489/a8b74873-8f7c-4fb8-adf9-68c7da0d0c6f.png'
		}
	];
	import Blog from '../../components/Blog.svelte';
</script>

<section class="flex p-3 flex-col">
	<h2
		class="font-semibold p-4 text-2xl sm:text-3xl md:text-4xl inline-block text-gray-100 hover:text-violet-300 transition-all duration-1000 ease-in-out cursor-pointer poppins border-b-2 border-transparent hover:border-violet-400"
	>
		Writeups? 📝
	</h2>
	<div class="grid mt-9 md:grid-cols-2 lg:grid-cols-3 gap-6">
		{#each blogs as blog}
			<Blog {...blog} />
		{/each}
	</div>
</section>
