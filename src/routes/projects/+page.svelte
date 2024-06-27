<script>
	import ProjectCard1 from '../../components/ProjectCard1.svelte';
	import ProjectCard2 from '../../components/ProjectCard2.svelte';
</script>

<section class="flex p-3 flex-col min-h-screen">
	<h2
		class="font-semibold p-4 text-2xl sm:text-3xl md:text-4xl inline-block text-red-300 hover:text-red-200 transition-all duration-1000 ease-in-out cursor-pointer poppins border-b-2 border-transparent hover:border-red-400"
	>
		Projects 🚀
	</h2>
	<h3
		class="text-center mt-3 font-light text-red-300 text-2xl poppins italic hover:text-red-400 hover:shadow-lg transition duration-300 ease-in-out cursor-pointer"
	>
		🐦‍🔥 Onchain Deployments 🐦‍🔥
	</h3>
	<div class="grid mt-9 md:grid-cols-2 lg:grid-cols-3 gap-8">
		<ProjectCard1
			imgSrc="/images/Artvault.png"
			title="🎨 Artvault "
			description="ArtVault, an art tokenization platform, enables direct sales of tokenized paintings, enhancing accessibility and transparency in the art market."
			githubRepoUrl="https://github.com/calc1f4r/Artvault"
			liveWebsiteUrl="https://artvault-mu.vercel.app/"
			youtubeLink="https://youtu.be/jkZFMKOzmIo"
		/>
		<ProjectCard1
			imgSrc="/images/ToudoList.png"
			title="⭕ Toudo List"
			description="A Web3 Todo List app using blockchain for secure, real-time task management on Sepolia Chain."
			githubRepoUrl="https://github.com/calc1f4r/Toudu-List"
			liveWebsiteUrl="https://toudu-list.vercel.app/"
		/>
		<ProjectCard1
			imgSrc="/images/BuymeAcoffee.png"
			title="🍵 Buy me a coffee"
			description="A Web3 implementation of 'Buy Me a Coffee', enabling direct support via blockchain transactions on the Sepolia Chain."
			githubRepoUrl="https://github.com/calc1f4r/Buy-me-a-Coffee"
			liveWebsiteUrl="https://buy-me-a-coffee-brown-one.vercel.app/"
		/>
	</div>
	<h3
		class="text-center mt-7 font-light text-green-400 text-2xl poppins italic hover:text-green-500 hover:shadow-lg transition duration-300 ease-in-out cursor-pointer"
	>
		🐍 Sec Python 🐍
	</h3>
	<div class="grid mt-9 md:grid-cols-2 lg:grid-cols-3 gap-8">
		<ProjectCard2
			title="🐚 Reverse Shell"
			description="Rev-Shell is a powerful Python tool for remote system management. Execute commands, transfer files, record audio, take screenshots, and more - all with an intuitive interface. Perfect for system admins, pentesters, or anyone needing remote control capabilities."
			githubRepoUrl="https://github.com/calc1f4r/Rev-Shell"
			playBackLink="https://www.youtube.com/embed/b6KI2r2HKpA"
			blogLink="https://hacklido.com/blog/656-python-for-hackers-10-building-a-reverse-shell"
		/>
		<ProjectCard2
			title="🌐 Network Scanner Tool"
			description="This Python script conducts network and port scanning using ARP ping, TCP, and UDP methods. Multithreaded for speed, it uncovers active hosts and open ports. Command-line customizable for your needs. 🔍🔒"
			githubRepoUrl="https://github.com/calc1f4r/Multithreaded-Network-Scanner"
			playBackLink="https://www.youtube.com/embed/bCLghkdWqxU"
			blogLink="https://hacklido.com/blog/642-python-for-hacker-5-building-a-mutlithreaded-network-scanner"
		/>
		<ProjectCard2
			title="🔥 Asynchronous FTP Bruteforcer"
			description="This is a Python script that implements an asynchronous FTP (File Transfer Protocol) bruteforcer. It utilizes asynchronous programming techniques to efficiently perform password guessing attacks on FTP servers."
			githubRepoUrl="https://github.com/calc1f4r/FTP-Bruteforcer"
			playBackLink="https://www.youtube.com/embed/ksvBP3pRKAQ"
			blogLink="https://hacklido.com/blog/526-python-for-hackers-2-ftp-bruteforcer-using-asynchronous-programming"
		/>
		<ProjectCard2
			title="🔥 SSH Bruteforcer using Asynchronous Programming"
			description="This tool is an asynchronous SSH brute-force script written in Python, designed to aid in testing the security of SSH authentication. It utilizes the power of asynchronous programming using the asyncio library and the asyncssh and paramiko libraries for SSH connections."
			githubRepoUrl="https://github.com/calc1f4r/SSH-Bruteforcer"
			playBackLink="https://www.youtube.com/embed/d7hcI4pCuzM"
			blogLink="https://hacklido.com/blog/525-python-for-hackers-1-ssh-bruteforcer-using-asynchronous-programming"
		/>
		<ProjectCard2
			title="🔥 Asynchronous Directory Buster"
			description="This tool is an asynchronous SSH brute-force script written in Python, designed to aid in testing the security of SSH authentication. It utilizes the power of asynchronous programming using the asyncio library and the asyncssh and paramiko libraries for SSH connections."
			githubRepoUrl="https://github.com/calc1f4r/Async-DirBuster"
			playBackLink="https://www.youtube.com/embed/meTjl3dy3Sk"
			blogLink="https://hacklido.com/blog/565-python-for-hackers-3-building-directory-buster-using-asynchronous-programming"
		/>
		<ProjectCard2
			title="🔥 Asynchronous Directory Buster"
			imgSrc="https://miro.medium.com/v2/resize:fit:877/1*IrusT9HxHYHOu_W7m4dWAg.png"
			description="This Python script leverages the power of the scapy library to perform ARP (Address Resolution Protocol) poisoning and packet sniffing on a local network. ARP poisoning is a technique where an attacker intercepts and manipulates network traffic between a victim and a gateway, effectively becoming a 'man-in-the-middle.',  also includes packet sniffing capabilities."
			githubRepoUrl="https://github.com/calc1f4r/Arp-cache-poison"
			blogLink="https://hacklido.com/blog/580-python-for-hackers-4-building-arp-spoofingposioning-script"
		/>
	</div>
</section>
