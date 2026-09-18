tryhackme Labs :-

\--------------

Pre Security Path :-

\-----------------

Offensive Security Intro Room :-

\-----------------------------

Task 1 :-

\-------

Think like a Hacker!

Offensive Security is about thinking like an attacker to find weaknesses before real hackers do.



In this room, you'll hack your first website in a safe and legal environment to see how ethical hackers operate.



Answer the questions below ---

Which term describes simulating a hacker's actions to find weaknesses?



Offensive Security

Defensive Security

Answer : Offensive Security

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 Lab :-

\----------

Starting the Lab

This room uses a virtual desktop to simulate a real system. A browser will automatically open, displaying FakeBank, a fake banking application. This is what you will be targeting.





View Site

Answer the questions below

What is the bank account number in the FakeBank application?



Answer :

\-------

Step 1 :-

\------

Click on the View site and it open the website in chrome browser.

Step 2 :-

\-------

Now one the top show bank account number simply just copy it 8881.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 Lab :-

\----------

Find Hidden Pages

Goal

Find a weakness in the FakeBank application. One common mistake is leaving hidden pages accessible.





View Site

Open the Terminal

Open the terminal on the machine. You will be using this to run your first hacking tool, dirbuster. The terminal icon looks like this:







&#x20;

Finding Hidden Pages

To find hidden pages using Dirbuster, we will use dirb and the URL that we wish to search:





dirb http://fakebank.thm

Any lines from the output that start with + are pages that have been found. Dirb will find two URLs.



Answer the questions below

Dirb found one URL, http://fakebank.thm/images.

What is the other hidden URL?

Answer :

\-------



Step-1 :-

\-------

We first run this in terminal dirb http://fakebank.thm and it scan this url

Step-2 :-

\------

Now we find the two pages after scan where one is already given in question http://fakebank.thm/images and another want which we get this website or page http://fakebank.thm/bank-transfer.



Scan Result by dribuster :-

\------------------------

DIRB v2.22

By The Dark Raver

\-----------------



\---- Scanning URL: http://fakebank.thm/ ----



\+ http://fakebank.thm/bank-transfer (CODE:200|SIZE:4663)

\+ http://fakebank.thm/images (CODE:301|SIZE:179)



\-----------------

END\_TIME: Thu, Sep 03, 2026, 21:02:16

DOWNLOADED: 4610 - FOUND: 2

Step-3 :-

\-------

Now the final result we get is this site http://fakebank.thm/bank-transfer

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



Task 4 Lab :-

\----------

Attack the Admin Page

You should now have found a hidden admin panel that lets you add money to your account.





View Site

To open this URL in the browser of the simulated desktop:



Add the following:

/bank-transfer

to the URL in the browser.

&#x20;



Use your account number 8881 and deposit $2000 (or more). After depositing, return to your account page and confirm the balance is now positive.



Answer the questions below

When your balance turns positive, a pop-up with green text appears.



Enter the green words as the answer (ALL CAPS)

Answer :-

\------

Step-1 :-

\------

First we open firefox and give this hidden url that we find in drib scan in our firefox browser http://fakebank.thm/bank-transfer.

Step-2 :-

\------

now we by the following question we give deposit amount is $ 2000 we can set more and give our bank account number that we get previously is 8881.

Step-3 :-

\------

Now we see the pop-up BANK-HACKED and we paste it and our lab is solve.

Step-4 :-

\------

Answer : BANK-HACKED

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



Defensive Security Intro :-

\-------------------------

Task 1 :-

\------

Think like a Defender

Think like a Defenderdepicting a person sitting at a desk, with multiple monitors stacked on one another showing various cybersecurity and data iconograhpy such as a map, bar charts, etc.

Defensive security is the process of defending and securing devices and systems.



Before you can defend a system, you need to understand what defenders are responsible for. Defensive security focuses on detecting and investigating attacks, and responding before damage occurs.



Unlike offensive security, you do not attack systems, instead, you monitor and protect them.



Answer the questions below

What is the main goal of defensive security?



Detect and respond to attacks

Attack systems to find flaws



Answer : Detect and respond to attacks

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 Lab :-

\-----------

Detect Suspicious Activity

Detect Suspicious Activity

Joe is an apprentice SOC analyst on his first solo shift. A moment ago, his monitoring dashboard lit up - something doesn't look right. Real SOC analysts rely on tools like this every day to separate normal activity from suspicious behaviour, and right now Joe needs your help to investigate before it becomes a serious incident.





View Site

This room uses a lab machine to simulate a real system.

Character

&#x20;

You'll need to...

1\. Open the monitoring dashboard

2\. Review recent alerts

3\. Identify the suspicious source IP.



Why you're doing this

Monitoring tools such as the one you'll be using provide insights as to what activity is taking place on computing devices. Defenders use tools like this dashboard to make sure that all activity taking place on these systems is legitimate, and investigate activity that is suspicious.



Answer the questions below

Which source IP address is generating the suspicious traffic?



Answer :

\-------

Step-1 :-

\-------

Click on view this site button.

Step-2 :-

\-------

There already give source ipv4 32.122.195.63 we copy it.

Step-3 :-

\-------

Now we give this source ip as a answer and our lab will be solve.

Step-4 :-

\------

Answer : 32.122.195.63

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3

Identify the Attack

Identify the Attack

Joe has spotted the suspicious activity, but knowing something is wrong is only half the battle. He now needs to figure out what the attacker is actually trying to do. The monitoring dashboard has been tracking every move, and the answers are in there.



Help Joe dig into the data and work out what kind of attack is underway before the attacker finds what they're looking for.





View Site

Character

&#x20;

You'll need to...

1\. Investigate the attack that has occured.

2\. View the "URL Discovery Attempts" list.

3\. Look at the latest "URL Discovery Attempts" entry to answer the question.



Why you're doing this

The monitoring dashboard shows a history of what the attacker is trying to find on our website. You will see that the dashboard has captured the attacker trying many attempts to access hidden pages, very quickly.



Once we know what the attacker is trying to achieve, we can then begin to take measures to stop the attacker and then finally fix the problem that allowed this attack in the first place.



Answer the questions below

Copy the latest URL that the attacker has tried to find and paste it below.

Answer :

\-------

Step-1 :-

\------

Now we see a dashboard where Web Discovery Attack which show informations are ---



Automated directory enumeration detected on admin endpoints

UNASSIGNED

\----------

MEDIUM

\------

Web Discovery Attack :-

\--------------------

Source IP

\---------

32.122.195.63

First Detected

\--------------

2 minutes ago

Event ID

\--------

SEC-000001



Attack Summary :-

\--------------

Attack Started

\--------------

14/07/2025, 10:21:39

Duration

\--------

16 minutes 32 seconds

URLs Attempted

\--------------

31

Blocked Requests

\----------------

10



URL Discovery Attempts :-

\-----------------------

GET 404 10:39:07 https://fakebank.com/admin -- here show copy url so we click on it



GET 403 10:35:05 https://fakebank.com/administrator



GET 404 10:37:44 https://fakebank.com/wp-admin



GET 404 10:37:04 https://fakebank.com/login



GET 200 10:37:23 https://fakebank.com/

Step-2 :-

\------

Now here after copy that url https://fakebank.com/admin and submit as a answer we see a prompt in the dashboard and our that lab will be solve.

Step-3 :-

\------

Answer : https://fakebank.com/admin

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 lab :-

\-----------

Stop the Attack

Stop the Attack

Joe knows who the attacker is and what they're trying to do. Now it's time to act. In defensive security, the immediate priority is containment (stopping the attack while it's happening) to protect the organisation.



For this stage of the practical, Joe has already completed some security updates, but needs your help to complete the last.





View Site

Character

&#x20;

You'll need to...

1\. Review the security actions. Joe has done two of these for you.

2\. Block the attacker's IP address below by adding it into the "Add Firewall Rule" textbox on the practical.

32.122.195.63



3\. Make sure to select "BLOCK" from the dropdown and press "Apply".

Why you're doing this

Answer the questions below

When the success message appears, copy the flag and paste it below.

Answer :

Step-1 :-

\-------

1\) Block Source IP Address

Block the IP address from the alert that is performing the web attack.



IP Address to Block

32.122.195.63

Block Duration (hours)

e.g. 24

Warning

This will immediately block all traffic from the specified IP address.



2\) Implement Rate Limiting

Set request rate limits for admin endpoints



Time Window (seconds)

60

Max Requests per Window

50



Step-2 :-

\------

Now we get that flag or answer in automatically in our font and we copy it and paste as a answer and we we that our lab is complete.

Answer : THM{FAKEBANK-SECURED}

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Careers in Cyber Room :-

\----------------------

Task 1 :-

\------

The Open Door

The jobs are already there. Are you?

There are millions of cyber security jobs sitting empty right now. Companies, hospitals, banks, and governments have created the roles but can't find the people to fill them.



Cyber security is open to anyone. From former police officers, healthcare workers, finance professionals to teachers and farmers, and much more. Cyber security needs people who understand how the world works, with unique skills, not just knowing how computers work.



Your background isn't a barrier to entry - it might be exactly what the industry is missing.



Answer the questions below

Which of these is true?



A) There are enough professionals to fill most roles



B) You need a computer science degree to get into cyber



C) Millions of roles are unfilled, and people from all backgrounds can fill them

Answer : C) Millions of roles are unfilled, and people from all backgrounds can fill them

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

What It Pays

Well paid. And faster to get there than you think.

Cyber security is one of the best paid fields in technology, and it doesn't require a decade of education to get there.



Entry-level roles pay competitively and Senior roles pay well. The right certifications and practice can take someone from no experience to a well-paying role in a significantly less time it takes to qualify in law, medicine, or finance.



No mandatory degree. No licence that takes years to earn. The barrier to enter cyber security is lower than most people assume, and the pay is good.



Answer the questions below

Which of these is true?



A) You need a four-year degree to be paid well in cyber



B) Certifications alone can get you to a well-paying role, faster than most people expect



C) Salaries are similar to general IT support



Answer : B) Certifications alone can get you to a well-paying role, faster than most people expect

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

The Bigger Picture

Protecting the things that can't afford to fail.

When hackers strike and cyber defences fail, the consequences can be critical. Hospitals cancel appointments. Banks freeze. Power grids go down, factories stop production, and personal information that's stolen has impact for years.



These things happen and are happening more often than ever before.



The people who stopped those attacks weren't just lucky. They knew what to look for, and they'd prepared for it. A team of experts, with the right knowledge, at the right moment, prevent serious incidents.



Answer the questions below

Which of these is true?



A) Cyber professionals protect hospitals, power grids, factories, and much more



B) Attacks only hurt the profits of an organisation



C) Cyber attacks only target tech companies

Answer : A) Cyber professionals protect hospitals, power grids, factories, and much more

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Find Your Place

There's a role for you in Cyber security

Cyber security isn't just one thing. It spans more than 50 recognised roles, from penetration testers and SOC analysts to threat intelligence researchers, incident responders, security engineers and beyond.





Some people in cyber think like attackers, testing systems for weaknesses before the wrong people find them. Others work like detectives, piecing together what happened after an incident. Some thrive on the "cat and mouse" of staying one step ahead of threats in real time. Others prefer the bigger picture, researching how threats evolve before anything goes wrong.



The skills that make people exceptional in these roles aren't just technical. The best problem solvers, the most calm people under pressure, the most curious, they often come from different careers entirely.



What matters is finding your place in this field that fits the way your mind works.



Answer the questions below

Which of these is true?



A) All cybersecurity roles require the same technical skills



B) There are many roles in cyber security, and the right one depends on how your mind works



C) Cyber security is a single career path, not a range of different roles

Answer : B) There are many roles in cyber security, and the right one depends on how your mind works

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\------

Your Starting Point

Every new technology needs someone to protect it.

Cyber security is one of the fastest growing career fields in the world and that growth shows no sign of slowing. AI, cloud computing, connected healthcare, digital banking, and much more. New technologies create more roles.



The people filling those roles don't come from one background, one degree, or one path. They start somewhere, usually with a question they couldn't stop asking. Neither do they stay in one place or role, they grow and expand their skills.



Answer the questions below

Which of these is true?



A) The availability of job roles is the same as other job markets



B) Cyber security is one of the fastest growing fields, and every new technology expands it further



C) AI will takeover Cyber security, requiring no one

Answer : B) Cyber security is one of the fastest growing fields, and every new technology expands it further

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Inside a Computer System Room :-

\------------------------------

COLD BOOT :-

\----------

CASE BRIEFING :-

\--------------

A workstation was pulled from a breach scene. The suspect was gone before anyone arrived. All you have is the machine, in pieces, and a case file with notes from the scene.



Some of the recovered components aren't from this machine. To rebuild it, you'll need to know what each part does, how it connects to the motherboard, and read the evidence closely enough to tell what belongs.



OBJECTIVE :-

\----------

Assemble the machine, boot it, find the evidence file, and email it to the senior analyst to close the case.



Step-1 :-

\-------

Hint idea Message what to do ---

Hi! Welcome to TryHackMe Forensics Labs.



This machine here came straight from a breach scene. The suspect was long gone by the time we showed up, but not before tearing the PC apart to slow us down. Our team collected everything they found at the scene and laid it out on that table. But here's the thing: some of those parts are impostors. Planted there just to confuse us.



What we do know is this: the machine only takes seven pieces. No more, no less.



So here's what you're gonna do. Check the evidence tags to learn what each component does. Figure out which seven actually belong. Rebuild the machine. Then recover the evidence file.



Once you've got it, email me the evidence flag.



And hey - if you get stuck, the case file's right there for a refresher. Or just hit the intercom and I can help you.

Step-2 :-

\------

Now here we have here many components those are -----

1. RAM :-

&#x20;  -----

|Random Access Memory (RAM)|CATEGORY : Memory|
|-|-|
|DESCRIPTION|1) Temporarily stores what the computer is working on<br />2) Makes data fast to access<br />3) Everything in it is lost when the power goes off|
|POSITION|DIMM slots on the motherboard<br />|



2\. Desktop Graphics Processing Unit (GPU) :-

&#x20;  ---------------------------------------

|Desktop Graphics Processing Unit (GPU)|CATEGORY : Visual Output|
|-|-|
|DESCRIPTION|1) Creates everything you see on the screen<br />2) Handles images, video and 3D graphics<br />3) Designed for a desktop machine|
|POSITION|PCIe x16 slot on the motherboard|



3\. Hard Disk Drive (HDD) :-

&#x20;  ----------------------

|Hard Disk Drive (HDD)|CATEGORY : Storage|
|-|-|
|DESCRIPTION|1) Stores files permanently<br />2) Keeps everything even when the power goes off<br />3) Uses spinning magnetic disks with moving parts|
|POSITION<br />|Drive bay inside chassis|



4\. Central Processing Unit (CPU) :-

&#x20;  ------------------------------

|Central Processing Unit (CPU)|CATEGORY : Processor|
|-|-|
|DESCRIPTION|1) Processes every program, click and instruction<br />2) Tells all other components what to do<br />3) Without it the computer cannot function at all|
|POSITION|CPU socket on the motherboard|



5\. Power Supply Unit (PSU) :-

&#x20;  ------------------------

|Power Supply Unit (PSU)|CATEGORY : Power|
|-|-|
|DESCRIPTION|1) Takes electricity from the wall socket<br />2) Converts it into the right voltage for each component<br />3) Nothing in the machine works without it<br />|
|POSITION|Mounted at the edge of the chassis|



6\. Solid State Drive (SSD) :-

&#x20;  -----------------------

|Solid State Drive (SSD)|CATEGORY : Storage|
|-|-|
|DESCRIPTION|1) Stores files, apps and the operating system<br />2) Keeps everything even when the power goes off<br />3) Fast, silent, no moving parts|
|POSITION|M.2 slot on the motherboard|



7\. Input/Output Panel (I/O) :-

&#x20;  -------------------------

|Input/Output Panel (I/O)|CATEGORY : Input / Output|
|-|-|
|DESCRIPTION|1) Contains all the ports on the outside of the machine<br />2) USB, HDMI, audio and ethernet live here<br />3) Everything you plug into the machine goes through this|
|POSITION|Rear I/O slot, at the edge of the chassis|



8\. Network Adapter :-

&#x20;  ----------------

|Network Adapter|CATEGORY : Connectivity|
|-|-|
|DESCRIPTION|1) Sends and receives data over a network<br />2) Sits inside the chassis not plugged in from outside<br />3) Without it the machine cannot go online|
|POSITION|PCIe x1 slot on the motherboard|



9\. Laptop Graphics Processing Unit (GPU) :-

&#x20;  -------------------------------------

|Laptop Graphics Processing Unit (GPU)|CATEGORY : Visual Output|
|-|-|
|DESCRIPTION|1) Creates everything you see on the screen<br />2) Handles images, video and 3D graphics<br />3) Smaller and lower powered than some graphics cards|
|POSITION<br />|Integrated into a laptop motherboard|



10\. USB Wi-Fi Dongle :-

&#x20;   ----------------

|USB Wi-Fi Dongle|CATEGORY : Connectivity|
|-|-|
|DESCRIPTION|1) Adds wireless internet to a computer<br />2) Connects the machine to a network<br />3) Works from outside the machine|
|POSITION|USB port on the outside of the chassis|



11\. Laptop Power Charger :-

&#x20;   --------------------

|Laptop Power Charger|CATEGORY : Power Supply<br />|
|-|-|
|DESCRIPTION|1) Converts the AC power from the outlet into the DC required by the computer<br />2) Plugs in from outside the machine|
|POSITION|External, connected to a wall outlet<br />|



Step-3 :-

\------

Now here we need to choose the 7 components to boot pc and find the evidence of case file ----



1. RAM
2. Desktop Graphics Processing Unit (GPU)
3. Central Processing Unit (CPU)
4. Power Supply Unit (PSU)
5. Solid State Drive (SSD)
6. Input/Output Panel (I/O)
7. Network Adapter



Step-4 :-

\-------

Now we click on the power on button and after that our windows system will be boot and need to go in evidence folder.



Step-5 :-

\------

Now there are several answers that we need to give ---



1. What is the primary function of Graphics processing unit (GPU) ?

Answer : Render Images and Visual Output to the screen



2\. What does the power supply unit (PSU) do ?

Answer :  Convert Mains electricity into the voltages each component needs



3\. What happens if central processing unit (CPU) is Missing ?

Answer :  Nothing executes - Machine cannot function at all



4\. What is the role of Motherboard ?

Answer : It connects and routes communication between all components



Step-6 :-

\------

Now we click on send to security analyst and then we click on the send mail and our lab will be solve.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Computer Types Room :-

\--------------------

Task 1 :-

\-------

Introduction :-

\-------------

Sophia was trying to connect a new device to her home’s WiFi when she noticed something unexpected: “NexusCool Fridge X17.” She laughed and wondered if connecting to the NexusCool Fridge X17 WiFi would let her download a cold meal. Setting the joke aside, she soon realized her neighbor had bought a smart refrigerator, a fridge with a built-in computer capable of connecting to the internet. It made her pause. Computers were no longer just laptops and phones. They were quietly infiltrating everyday objects, from kitchen appliances to doorbells. Sophia had seen strange stories online about smart devices behaving badly, but she had never really stopped to think about what these machines actually were.



She looked forward to learning more about computers during her upcoming summer internship.



Learning Objectives

Upon completion of this room, you will be able to identify and distinguish between different types of computers you use directly, such as laptops and smartphones, and indirectly, such as servers, IoT devices, and embedded systems. You will also understand what makes each type suited to its purpose.



Answer the questions below

Ready to find the hidden computers?

Answer : yes we ready

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Sophia’s Summer of Hidden Computers – Month 1 :-

\-----------------------------------------------

The Computers You Sit in Front Of

During her first month at Nova Labs, Sophia learned an important lesson.



Character :-

\----------

&#x20;

Sophia learned that...

1\. Not all computers are meant to move.

2\. Not all computers are meant for people to sit in front of.

She was introduced to four types of computers that often look similar but serve very different purposes.



Portable everyday computing

Sustained performance at a fixed location



Let's compare these below:

\-------------------------



|Computer Type|Screen and Keyboard|Main Purpose|
|-|-|-|
|Laptop|Yes|Portable everyday computing.|
|Desktop|Yes|Sustained performance at a fixed location.|
|Workstation|Yes|Precision and reliability for professional tasks.|
|Server|No|Providing services to many users over a network.|



How Sophia Learned the Difference :-

\---------------------------------

Sophia began with a laptop, the computer she already knew best. It was perfect for emails and documents, but when she pushed it with long tasks, it slowed down. Gabriel explained that laptops are built to be portable, and staying cool in a small, battery-powered device is difficult.



Next, she tried a desktop. It stayed in one place, used wall power, and had better cooling. The same task ran smoothly for much longer. Desktops are designed for consistency rather than mobility.



When Sophia moved on to professional work, such as simulations and 3D models, Gabriel showed her a workstation. It looked like a desktop, but it was built differently. Workstations prioritize accuracy and reliability, using specialized components to reduce errors during long or complex computations.



Finally, Gabriel took her to a room full of machines with no screens at all. These were servers. They ran continuously, answering requests from multiple users simultaneously. Sophia never touched them directly, but they powered the tools she used every day.



Answer the questions below

1. Which computer type usually runs without a dedicated screen and keyboard?



Answer : Server

\------

2\. What kind of computer with specialized components would one buy to carry out precision work?



Answer : Workstations

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

Sophia’s Summer of Hidden Computers – Month 2 :-

\----------------------------------------------

By her second month at Nova Labs, Sophia had started noticing computers she had never interacted with directly. The most powerful computer most people own fits in their pocket, but millions more hide inside everyday objects: doors, lamps, coffee machines.



We continue to find computers hiding in everyday objects:

\--------------------------------------------------------



|Type|What it is|Examples|
|-|-|-|
|Smartphone|Pocket-sized computer optimized for battery life and connectivity|iPhone, Android phone|
|Tablet|Touch-first computer with larger screen|iPad, drawing tablet|
|IoT device|Network-connected device with a single purpose|Thermostat, smart doorbell, fitness tracker|
|Embedded computer|Computer built into another device|Coffee maker controller, automatic door sensor, lamp dimmer chip|



IoT vs Embedded:

\---------------

Both can be small and single-purpose. The difference is connectivity. IoT devices connect to a network to report data or receive commands. Embedded computers might not connect to anything; they do their job inside the machine, often for years without anyone knowing they exist.



Sophia walked through automatic doors every day at Nova Labs. She never realized that a tiny computer inside the door frame was detecting her movement and signaling the motor to open. That’s embedded computing; invisible, reliable, everywhere.



Answer the questions below

What is the currently most popular pocket-sized computer?



Answer : Smartphone

\-------

What kind of computer would you expect to find in a coffee machine?



Answer : Embedded computer

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Why Computers Come in Different Flavors

Sophia asked the question that had been bothering her all summer:



Character

&#x20;

Sophia asked...

Why not just build one computer that does everything?

“Because every design is a trade-off,” replied Gabriel.



Mobility costs power. Smaller, portable computers must sacrifice sustained performance. Reliability costs money. Servers and critical systems use redundancy, such as extra power supplies and disks, to avoid failure.



Purpose shapes everything. You touch a phone. You ask a server for information. An IoT device works quietly without demanding attention.



There is no best computer. There is only the right tool for the job!



Click the View Site button below, then complete the interactive challenge to get the flag.



Step-1 :-

\-------

we found 8 computers in a room like smart tv, robotvacuum, smart watch, smart fridge, smart speaker , security cam, wifi router, thermos stat.

Step-2 :-

\------

Now we see the cooling difference between laptop and desktop

|LAPTOP|DESKTOP|
|-|-|
|1) Tiny Fan|1) Large Fan|
|2) Heat Pipes|2) Airflow space|
|3) Heat Sink|3) Tower cooler|
|Result : Throttles under load|Result : Sustained Performance|



Step-3 :-

\------

Gabriel takes Sophia to the server room. Rows of machines hum quietly, lights blinking. "These servers run our entire business 24/7," Gabriel explains.



"What happens if the power goes out?" Sophia asks. Gabriel smiles. "Great question. Try disconnecting the power supplies and find out."



GOAL

Test all three power scenarios: both on, one off, and both off.



1. Here user to redundant power that reduces a single failure point ( two power connection use suppose A and B Both) so server run.
2. Now suppose in A and B power cable one is goes off then one still up and supply power so still server run.
3. both suppose power connection A and B off and power supply goes off then the server offline and goes off and unavailable.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

step-4 :-

\------

At the end of the day, Gabriel gives Sophia a final challenge. "Now that you know about different computer types, let's see if you can match them to real jobs."



"Every computer exists because of specific tradeoffs," Gabriel explains. "Match each task to the computer type that handles it best."



GOAL

Match all 3 jobs to the correct computer types.



1. Edit 4k video all day by using workstation pro hardware
2. Host a website 24/7 by using Server that is always on
3. Ring when button pressed by using Embedder that design for one job

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

step-5 :-

\-------

Sophia has completed her training. Gabriel gathers the team to celebrate her first week at Nova Labs.



"You've learned about laptops, desktops, servers, phones, embedded systems, workstations, and IoT," Gabriel says. "Let's see what you remember!"



GOAL

Score at least 4 out of 5 on the final quiz.



Question 1 of 5 :-

\---------------



1. Why do laptops throttle more than desktops?



A) Smaller batteries



B) Less cooling space



C) Weaker WiFi



D) Older processors

Answer : B) Less cooling space



2\. What does server redundancy prevent?



A) Faster speeds



B) Single point of failure



C) Higher costs



D) More storage

Answer : B) Single point of failure



3\. Why do smartphones last longer on battery than laptops?



A) Bigger batteries



B) Optimized for efficiency



C) Fewer apps



D) No screen

Answer : B) Optimized for efficiency



4\. Which feature is more common in workstations?



A) RGB lights



B) ECC RAM and certified drivers



C) Faster WiFi



D) Bigger case

Answer : B) ECC RAM and certified drivers



5\. In many smart homes, what coordinates devices?



A) Smart light



B) Thermostat



C) Hub or cloud service



D) Camera

Answer : D) Hub or cloud service

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



Client-Server Basics Room :-

\--------------------------

Task 1 :-

\------

Introduction :-

\------------

In the previous rooms, we looked at different types of computers and how computers are used at work. Initially, most computers worked alone: they stored their own files, ran their own programs, and did not communicate with other computers.



Soon, multiple organizations around the world started with the idea of interconnecting these systems to facilitate information exchange and resource sharing regardless of distance. Hence, the precursors of the "internet" were born. Networks such as ARPANET, CYCLADES, NPL, and NSFNET paved the way for the modern internet.



Just like in society, where people distinguish themselves with a particular set of skills and offer these as a service, interconnected systems started to specialize as well. So how does this work? How are computer systems able to use services on another computer system? At the end of this room, you will know the answer to these questions.



Learning Objectives :-

\--------------------

Understand the Client-Server model

Understand the following concepts on a surface level:

DNS

Client

Server

Port

Protocol

Network

Prerequisites

Coming soon: Inside a Computer System

Coming soon: Types of Computers

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

Pizza Delivery, One of the easiest ways to explain how computer systems provide services to other systems is to use an analogy: for example, how shops offer services to their customers. Let's have a look at a pizza takeaway.



It's Friday night, and Alice and Bob feel like having pizza. Alice looks at Luigi's Pizza's menu and tells Bob which pizza she wants. Bob takes the car, enters Luigi's address into his GPS, and starts driving. Once Bob arrives, he enters Luigi's and places his order: "Get me a large pepperoni pizza and a coke." The employee acknowledges the order and starts making the pizza. Once the order is ready, Bob returns home and has a lovely pizza night with Alice.



This seems like a standard, straightforward process. But don't be fooled. Because we are so used to ordering pizza, we have internalized the process. Let's have a closer look at each step and relate it to how computer systems interact.

Service, Client, Server

In our analogy, Bob and Alice choose to use the Pizza takeaway service. Alice is the client who passes her order to Bob, who then passes it to the Server at Luigi's Pizzas. In computer terms, we can translate this as Alice using, for example, a browser to navigate to a website. The browser is the client that requests the webpage, and the server is the system that serves it.



Note that the client is the one who always initiates the request.



Request and Response :-

\---------------------

Alice requested a large pepperoni pizza from Luigi's. Be careful, this request was not made to Bob. Bob was the one who brought the request to Luigi's. What is important to realize is that if the request is not formatted correctly or the requested resource is unavailable, we will get an error response. For example, Bob returns to Alice with the message that there were no pepperoni pizzas or that the server did not understand the order.



In computer systems, we can say that Alice used a browser (the client) to request a webpage from a server, which then sent the webpage to the client.



Protocol :-

\--------

One of the things we don't often realize, until we go on a trip to a foreign country, is our language. When Alice formulates her request to Bob, she uses the language Luigi's Pizza understands. Additionally, Alice uses the menu to determine which orders she can place. Bob understood the request (language and order) and went to Luigi's to bring it; he received a response he understood and brought it back to Alice.



We can compare Bob to a protocol that computer systems use to communicate. A protocol defines how a client can communicate with a server. This definition includes:



1. Which commands do the client and server understand. E.g., the get command.

2\. How a request is structured. E.g., first the command and then the order.

3\. What syntax is used. E.g., Alice uses the English language.

4\. What response should be given to which type of request. E.g., a request for pizza results in receiving the available pizza.

5\. What response to give to faulty requests. E.g., the server at Luigi's Pizzas says: No pepereonni pizza available

Port

A port is used to identify a specific service running on a system. When a client wants to access a service on a server, it must connect using the correct port.



Imagine that Luigi’s takeaway service requires customers to enter through a specific door. Everyone ordering takeaway uses the same door. In the same way, a service on a server listens on a specific port.



Now imagine that Luigi’s offers multiple services, such as takeaway, dining in, and delivery. Each service uses a different door: door A for takeaway, door B for the restaurant, and door C for delivery. Similarly, a single server can run multiple services at the same time, with each service identified by a different port.



DNS :-

\---

When Alice sent Bob her request, only the name of the pizza place was known. With that alone, it is not possible to reach the destination. So, Bob entered Luigi's Pizza into a GPS device, and the device returned the coordinates for Luigi's.



DNS stands for Domain Name Service and works similarly to GPS: when you enter the name of, for example, a website, DNS resolves it to server's location. These location coordinates are called an Internet Protocol (IP) address in computer terms. Imagine this IP as the address to your home (street name, house number, postal code, city, and country), but for computer systems.



Let's look at the next task to see how the client-server model applies when browsing a website.



Answer the questions below

1. What do we use to identify a specific service on a server?



Answer : Port



2\. What do we call the address of a server?



Answer : Internet Protocol Address

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 lab :-

\-----------

Web Communication in Practice :-

\-----------------------------

Hypertext Transfer Protocol (Secure), abbreviated as HTTP(S), is a stateless client-server protocol used for the World Wide Web. This means that each request is processed independently, without the server retaining information about previous requests.



Although the protocol itself is stateless, modern websites and web applications implement mechanisms to introduce statefulness at the application level.

For example, when you log into a website using your credentials, the server creates a session identifier (often stored in a cookie or token) that is sent with each subsequent request.

Without these mechanisms, you would need to authenticate again with every new request, because the server would have no memory of your previous login.



HTTP Commands :-

\-------------

In the main specifications that define HTTP (also called Request for Comments, or RFC documents), there are 9 core commands. In HTTP lingo, we use the term method instead of command. Below you can see an overview of these methods:



GET

POST

PUT

DELETE

PATCH

HEAD

OPTIONS

CONNECT

TRACE

We will focus on discussing one of the two most common methods used: GET. We will approach this practically by examining the requests a browser sends when you navigate to a website.



Click on the "Start Lab Machine" button below. This will show a new window in split-screen where we can open a website and inspect a GET request. If the split-screen is not showing, click the blue "Start Split-screen" button at the top of the room.



GET :-

\----

The GET method is actually pretty straightforward. We can use this method to retrieve a resource from web server. For example, GET https://tryhackme.com/index.php. This request retrieves the TryHackMe website's homepage. You don't need to type in this request yourself. When you open a browser (this is the client) and type "https://tryhackme.com," the browser constructs the message behind the scenes using information you provide and other fields defined in the HTTP specifications. When the web server receives the request, it sends a response that includes a status code (Indicating the type of response) and the requested information. The image below shows the flow of this request.



Let's have a look at an actual GET request and its response. Navigate to the Lab Machine that opened next to this screen, then click the Firefox icon on the Desktop. Once the browser is open, the web page http://httpdemo.local:8080 should show. Proceed by pressing F12 or right-clicking in the browser window and selecting "Inspect". This will open the Firefox Developer Tools, which allows us to inspect, debug, and analyze web pages and traffic. Click on the "Network" tab as shown in the image below.



Now reload the page by clicking the circular logo highlighted on the image above (next to where you type the URL). You should see multiple GET requests appearing in the Developer Tools window, under the Network tab. Click on the first entry as shown below to see more information.



In the right-hand panel, we can see more information about our GET request. We won't go into much detail, but let's have a look at some of these fields.



Scheme: Tells us which protocol was used: HTTP or HTTPS.

Host: Tells us the name of the host we request resources from.

Filename: Indicates which file we requested from the host. In our request, this is "/", which actually translates to "index.html".

Address: Displays the IP address where the website is hosted. In our example, we are hosting the website on the same device. That's why the address 127.0.0.1 is shown.

Status: This field indicates whether the request was successful. In our example, we received a "200 OK" status, which means that the request was successful.

When a request is sent, we will get a response from the server. The response is divided into two parts: the response header and the response body. The response header contains metadata about the response, while the response body contains the requested content.



We can see this response body by clicking on the "Response" tab when displaying the details of a request. In our example, the response contains the index page of the requested website. The image below shows the content in HTML format.



Conclusion :-

\----------

In this room, we have explored how devices on the internet can offer services to each other. We focused on the client-server model, which is similar to ordering a pizza. The client initiates the communication and the server replies.



Then, we continued with an example of the HTTP protocol which is used for websites. We saw a practical example of how a client request and server response actually looks like behind the scenes.



Now that we have seen how services are offered on the internet, let's have a look at the infrastructure that supports them. In the next room we will cover the basics of virtualization.



LAB Steps :-

\----------

Step-1 :-

\-------

first we open firefox and give this http://httpdemo.local:8080/ and press enter.

Step-2 :-

\-------

here we this interface ------

&#x20;http://httpdemo.local:8080/

HTTP GET Request Demo



If you open DevTools → Network, you will see:



&#x20;   index.html or '/'

&#x20;   style.css

&#x20;   script.js

and now we see click button we press on click me button.

Step-3 :-

\------

now it popup and show in screen when click button --

httpdemo.local:8080

JavaScript loaded via GET!

Step-4 :-

\------

Now we right click and then click on inspect button and then to Network tab and reload the page and see the GET method and 200k status like example ----------



1. GET

scheme :http

host : httpdemo.local:8080

filename : /



2\. GET

scheme : http

host : httpdemo.local:8080

filename : /style.css



3\. GET

scheme : http

host : httpdemo.local:8080

filename : /script.js



4\. GET

scheme : http

host : httpdemo.local:8080

filename : /favicon.ico



note :-

\----

in scheme there are set the protocols that used in web application like it can be http or https. host is teh website or domain name and file name is the name of the frontend file.

Step-5 :-

\------

Now we give the following questions answer ----

1. What would be the host in the following URL https://www.iamlearning.thm/contact ?



Answer : www.iamlearning.thm



2\. What would be the scheme in the following URL https://www.iamlearning.thm/contact ?



Answer : https

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Virtualisation Basics Room :-

\---------------------------

Task 1 :-

\------

Introduction :-

\-------------

In previous rooms, you learned what the components of a computer are and how they communicate with each other. In this room, you will learn how companies have optimized these computer components to reduce costs and build flexible, scalable systems that power the modern internet through a concept known as virtualization.



Have you ever considered how expensive and inefficient it would be if every piece of software or every website required its own physical server?

Virtualization was created to solve exactly this problem.



Illustration with multiple virtual computers pointing to a physical server.



Your manager asked for help on improving the hardware utilization of a computer that hosts a website. Let's explore the concept of virtualization and help your manager!



Learning Objectives :-

\--------------------

1. Understand why managing applications on individual physical servers is inefficient.

2\. Learn how virtualization addresses hardware utilization and scalability challenges.

3\. Understand the components of a lab machine.

4\. Learn how containers have further optimized hardware utilization for applications.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

Virtualization Overview :-

\------------------------

Before the concept of virtualization, the rule of thumb in IT was:

“One server = one application.”



In the early days, digital services were run on physical machines, and each machine typically had a single, clear purpose, such as hosting a website or storing data. As businesses added more services, they naturally increased the number of physical servers, and the “one job per box” approach became the standard for building reliable systems.



This meant that if a company wanted to run a website, a database, an email service, and an internal app, they would need separate physical servers for each one. The problems were obvious:



High cost: Buying multiple physical servers is expensive, not just the hardware, but also electricity, cooling, maintenance, and data center space.

Low utilization: Most applications don’t use the server’s full capacity. Many servers stayed at 5–20% usage, wasting CPU, memory, and storage resources.

Slow deployment: Setting up new physical servers could take days or weeks.

Hard to scale: If an application suddenly needed more resources, you often had to buy yet another server.

In short, companies were paying a lot for hardware that wasn’t being fully utilized.



Illustration of how costly it was to have multiple physical servers for each application.



The Need for Sharing Hardware Safely and Efficiently

Virtualization introduced a new idea:

“What if multiple applications could share the same physical server safely?”



A virtualization layer, called a hypervisor, was introduced to act as a referee between lab machines and allow each virtual computer to behave independently, like a physical computer.



The Building Analogy

Imagine if one single person lives alone in an entire 10-floor building:



The person uses only one floor but must maintain the entire building: electricity, cleaning, water, and security.

Most of the building stays empty and wasted.

It’s expensive, inefficient, and unnecessary for his needs.

Now imagine dividing the building into separate apartments:



Each apartment has its own door, walls, kitchen, and privacy.

Different people can live independently without bothering each other.

They all share the building’s main structure: electricity, water, and elevators, making it cheaper and more efficient for everyone.

Illustration of building analogy. The first building has multiple empty apartments, indicating the wasted resources. The other building has a building manager, representing the hypervisor and multiple apartments, representing the lab machines. This is virtualization:



The building = the physical server

The apartments = lab machines

The tenants = applications or operating systems

The building manager = the hypervisor (the software that divides the building safely)

Each virtual computer, known as a Lab Machine (VM), acts as an independent system with its own operating system, apps, and settings, even though they all share the same physical hardware underneath.



Answer the questions below:

What does virtualization enable multiple applications to share?



Answer : Physical Server

\------



What is the name of the software that manages the resources for each lab machine?



Answer : Hypervisor

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

Virtualization Components :-

\-------------------------

Hypervisor (The Building Manager) :-

\---------------------------------

A hypervisor is the core technology behind virtualization. It's the software that creates and manages lab machines.



It is a special piece of software that:



1. Divides a physical computer into multiple virtual ones.

2\. Gives each lab machine its own share of CPU, memory, and storage.

3\. Keeps everything isolated and safe.

4\. Manages the lifecycle of lab machines (start, stop, pause, clone, delete).

5\. Hypervisors have two main types of implementation, each of which is used for specific scenarios, from home labs to large data centers:



* Type 1 hypervisors run directly on the physical hardware, making them fast, efficient, and ideal for servers and professional environments.
* Type 2 hypervisors run within an existing operating system, making them easier to install and ideal for learning, testing, or small setups.

Below is a table showing which use case is best suited to each hypervisor type. The use cases can run on both hypervisor types, but it's not the best approach given the main objectives of each.

|Use Case|Type 1|Type 2|
|-|-|-|
|Test Malicious Files||X|
|Production Server|X||
|Database Server|X||
|Software Testing||X|
|Kali Linux||X|
|Data Center|X||



When using virtualization to test malicious files, care should be taken to ensure that the host machine does not become infected by the malware being tested in the guest machine. One approach is to use different operating systems for the guest and host machines, or to isolate the guest machine so that it does not communicate with the host.



Lab Machines (The Apartments) :-

\------------------------------

A Lab Machine (VM) is a virtual computer created by the hypervisor.



Even though it’s virtual, it behaves as a real machine:



1. It has its own virtual CPU, RAM, storage, and network.

2\. It can run any operating system (Windows, Linux, etc.).

3\. It’s completely isolated from other VMs. This means that if one VM breaks, the others continue to work.

4\. You can deploy VMs on your own computer using tools such as Oracle VirtualBox and VMware Workstation. This type of software acts as a type 2 hypervisor and lets you run multiple operating systems, such as Windows, Linux, and macOS.



Since you have learned what a hypervisor and VM are, let's take some examples where you might need them:



You need to work on a different OS like Kali Linux, but you can't buy another whole system, so you install a hypervisor and run a Kali Linux VM on it.

You want to test whether a file is malicious, so you set up an isolated lab machine to protect your main computer from being infected.

Containers (The Rooms Inside the Apartment)

A container is a lightweight, isolated environment that runs a single application and all the necessary components to support it. Instead of bringing a whole separate operating system, a container borrows the core of the existing system by running on the kernel, which is the part of an operating system that communicates with the hardware and manages resources such as memory and running programs.



Because containers share this kernel, they start quickly and use fewer resources than full lab machines, but it also means they must match the host system’s type. For example, you can’t run a Windows container on a Linux machine.



Containers behave like small, self-contained spaces because:



1. They package the application and its dependencies (libraries, tools, versions).

2\. They share the host’s operating system, so they start almost instantly.

3\. They remain isolated from each other, so a misbehaving container doesn’t affect the others.

4\. They can run consistently on any machine, making them perfect for development, testing, and scalable deployments.

5\. The easiest way to deploy containers in a VM is using Docker.

6\. Docker is an open-source software platform that simplifies the process of building, deploying, and running applications using containerization.



The image below illustrates the relationship between Hypervisors, VMs, and containers:



Diagram showing a physical server with a hypervisor, two lab machines, and two containers running inside one VM.



In summary, VMs provide the “full apartment” with maximum separation and flexibility, while containers offer lightweight “rooms” ideal for scalable, fast-deploying applications.



Answer the questions below :

1. Suppose a user wants to deploy a study lab on their machine to practice some exercises for a cyber security certification. Which type of hypervisor will they use?



Answer : Type 2



2\. Suppose a company wants to host multiple small applications in the same lab machine. What should they use?



Answer : Containers

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Managing Virtual Machines :-

\-------------------------

After learning about virtualization, you were hired to be responsible for the virtual environment for AutoGalo, a company that has recently started using lab machines.

In this company, they use an application called Virtualization Manager. This application provides a clear view of the overall status of an entire virtualization environment, providing details of each virtualized instance and the physical hosts. It also enables you to run actions and manage the VMs you create.



Your manager has asked you to investigate an issue with the email service. Essentially, everyone in the company stopped receiving emails today, and no one knows what happened.



Summary: Provides a generic view of the state of the environment.

Lab Machines: Provides details of each VM and enables you to run actions on them.

Hosts: Displays usage and performance details for each physical server.

Go to the Lab Machines section and look for the VM with the name Mail-SERVER:



Lab Machine section screenshot highlighting the Mal-SERVER machine.



Looks like this lab machine has entered an Error state. Let's try rerunning this VM using the Blue Square Button to restart it.



Lab Machines section screenshot highlighting the restart button.



After running again, it appears to be working correctly, with no errors!



Creating a Lab Machine

As part of your routine, you create lab machines for other teams. After resolving the email server issue, you received a task to create a VM to support the marketing team's website.



Now, let's create a VM to host their marketing website. In the Lab Machines section, locate the + Create VM button on the top right side of the Lab Machines section and click on it.



Lab Machines section screenshot highlighting the "+ Create VM" button.You should fill out the form with how much hardware your lab machine will be using:



Name: Marketing-VM

CPU Cores: 4

Memory (GB): 8

Disk Size (GB): 100

Then click on Create VM



Screenshot of the form to create a VM.

Now, at the top of the list of Lab Machines, you should see your created VM:



Lab Machines section screenshot highlighting the new Marketing-VM created.



Analyzing Hardware Usage

Another routine task you have is to manage the health of the physical servers and report status to your manager. Go to the Hosts section at the bottom of the page:



Screenshot of Hosts section.

By analyzing it, we can identify:



1. HV-PROD-01 has the capacity to host more VMs.

2\. HV-PROD-02 is almost operating at 100% of its capacity, and we might need to report this!

3\. HV-BACKUP-01 is disconnected and does not host any VMs.

4\. Hosts section screenshot highlighting the insights mentioned above.



Step-1 :-

\------

There we see that by using the virtual manger we see all virtual environment status there we see that mail\_SERVER name machine status show error so there we click on the restart(recover) button and then the server status change to running.

step-2:-

\------

Now we click on add new vm button and then click on create VM button with this specification where ----

Name: Marketing-VM

CPU Cores: 4

Memory (GB): 8

Disk Size (GB): 100

Sep-3:-

\------

Now we see that our new VM named Marketing-VM appear which status currently show stopped.

Step-4 :-

\-------

Now the next task we have that we see this VM capacity where -----



|VM Name|CPU usage percentage|storage usage percentage|memory usage percentage|number of VM|System status|
|-|-|-|-|-|-|
|HV-PROD-01|45|72|68|3|Connected|
|HV-PROD-02|98|95|90|8|Connected|
|HV-BACKUP-01|0|30|0|0|Disconnected|



* HV-PROD-01 has the capacity to host more VMs.
* HV-PROD-02 is almost operating at 100% of its capacity, and we might need to report this!
* HV-BACKUP-01 is disconnected and does not host any VMs.



Now, answer the following task questions to conclude your shift as the responsible for virtualization in AutoGalo!



Answer the questions below:

What is the name of the lab machine that has been running for the longest time?



Answer : Monitoring-SYS (6 weeks is it uptime)



What is the name of the lab machine that is using the biggest amount of memory?



Answer : DB-Cluster-01 (32 GB use)



How many VMs are in the running state after you solved the issue on `Mail-SERVER`?



Answer : 8



What is the name of the physical machine that is hosting most of the VMs?



Answer : HV-PROD-02 ( 8 VM it have)

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\-------

Conclusion :-

\-----------

In this room, you learned why virtualization is such a critical foundation in modern IT, both for maximizing hardware efficiency and for safely isolating environments.



Key Terminology :-

\---------------

Let's quickly review some concepts we learned in this room:



1. Virtualization:

\---

Enables a single physical computer to act like multiple separate computers.



2\. Hypervisor:

&#x20; -----------

The “manager” software that makes and runs the virtual computers.



3\. Lab Machine (VM):

&#x20;  ----------------

A whole virtual computer inside the real one, with its own system.



4\. Container:

&#x20;  ---------

A small, isolated box for one app that shares the same system as the host.



5\. Container Images:

&#x20;  ----------------

A pre-packed recipe/template used to create containers.



6\. Network Ports:

&#x20;  -------------

Special numbered entry points that apps use to talk over the network.



We also concluded that the key benefits of virtualization are:



* Cost savings
* Better resource usage
* Safe testing for cyber security
* Faster deployment
* Flexibility
* Portability
* Scalability
* Centralized Management



Further Learning :-

\----------------

Through hands-on practice, you experienced how virtualization simplifies and accelerates application deployment, providing a fast and secure way to run applications consistently.



With these fundamentals, you are ready to explore the Cloud concept in the Cloud Computing Fundamentals room, which uses virtualization, containerization, and automation to provide scalable, on-demand services!

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Cloud Computing Fundamentals Room :-

\----------------------------------

Task 1 :-

\-------

Introduction :-

\-------------

Imagine you have a fantastic idea for an app that helps students practice cyber security, and you host it on your own computer in your country. But what can you do when users from other parts of the world try to access it and experience lag? What if many students connect at the same time, or your computer is turned off? These limits make it hard for the app to grow.

That's when cloud computing comes to play and solves these problems!



The cloud is built on top of technologies you already learned, like virtualization and containers. These enable running many applications efficiently on shared infrastructure and quickly creating or changing environments when needed.



Illustration of multiple devices connected to a Cloud.



In this room, we will explore the basics of cloud computing and how this impacts the way modern applications are built, deployed, and used every day.



Learning Objectives :-

\-------------------

* What is cloud computing
* Service models of cloud (IaaS, PaaS, SaaS)
* Cloud Types (Private/Public/Hybrid)
* Benefits of cloud computing
* How big companies are using the cloud

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Cloud Computing Overview :-

\-------------------------

Cloud computing is the perfect solution for the challenges in the application you’ve designed, such as moving your files from a single laptop to online storage that you can access anywhere. Instead of running your app on one computer in one country, the cloud lets you use computing resources over the internet. This makes your application easier to access, more reliable, and ready to grow as more students start using it.



How Servers Evolved to Cloud :-

\----------------------------

Before we start diving into cloud details, it’s helpful to understand that cloud computing did not appear suddenly. It is the result of many years of changes in how servers were used and managed. At each step, businesses looked for ways to reduce costs, use resources more efficiently, and make their applications easier to run and scale. The timeline below shows this evolution, from physical servers to the cloud we use today:



Timeline illustrating the evolution from physical servers to the modern cloud era.



Cloud Benefits and Characteristics :-

\-----------------------------------

After seeing how applications evolved from physical servers to the cloud, it's becoming clear why cloud computing is so widely used today. The cloud was designed to address common problems, including limited capacity, high costs, and slow growth.

The following benefits and characteristics explain how cloud computing makes applications easier to run, scale, and manage:



Scalability :-

\-----------

* Easily scale up or down as your application's needs change.
* On-demand self-service:-

&#x20;  -----------------------

Create or remove servers and storage instantly, without waiting for hardware.

* Pay only for what you use:-

&#x20;  --------------------------

You are charged based on usage, not upfront costs.

* Security:-

&#x20;  ---------

Cloud providers protect the infrastructure with strong security measures.

* High availability:-

&#x20;  -----------------

Applications keep running even if part of the system fails.

* Global access:-

&#x20;  --------------

Your application can be accessed by users anywhere in the world.



In simple terms, the cloud enables IT resources to be flexible, cost-effective, and easier to manage.



Types of Cloud :-

\--------------

The flexibility provided by cloud computing allows applications to be run in different ways, depending on your needs and level of control. Because of this, cloud providers offer multiple models for deploying and using applications, each suited to different scenarios.



Let’s start with the deployment types you can choose for a cloud environment:



1. Public Cloud :-

&#x20;  ------------

Used by startups, websites, and global apps because it is affordable, easy to scale, and requires no infrastructure management. Public cloud services are preferable for nearly every use case.

2\. Private Cloud :-

&#x20;  --------------

Used by banks, healthcare, and government organizations because it offers greater control, customization, and compliance for sensitive data.

3\. Hybrid Cloud :-

&#x20;  ------------

Used by companies like e-commerce platforms that need to keep sensitive data private while still scaling publicly during high demand.

Just like there are different ways to deploy a cloud environment, there are also different ways to use cloud services. Depending on your experience and needs, you can choose the level of responsibility that fits your application.



cloud service models:-

\--------------------



1. Infrastructure as a Service (IaaS) :-

&#x20;  ----------------------------------

You rent basic computing resources such as virtual servers, storage, and networking. You are responsible for managing the operating system and your application, while the provider manages the physical hardware.

2\. Platform as a Service (PaaS) :-

&#x20;  ----------------------------

The cloud provider manages the infrastructure and the operating system. You focus on building, deploying, and running your application without worrying about servers.

3\. Software as a Service (SaaS) :-

&#x20;  ----------------------------

You use a complete application over the internet. The provider manages everything, and you access the software through a browser or app, for example, Gmail or Zoom.

Think of cloud service models like different ways of renting a place to live:



An analogy image showing how cloud service models can be compared to renting an apartment.



Major Cloud Vendors

There are several cloud vendors offering a variety of services, but Amazon Web Services (AWS) is the industry leader, with the most extensive offerings and global reach. Other well-known cloud providers include:



1. Microsoft Azure:-

&#x20;  ----------------

A strong competitor, especially in enterprise and hybrid cloud environments.



2\. Google Cloud Platform (GCP):-

&#x20;  ---------------------------

Known for powerful data analytics, AI, and machine learning tools.



3\. Alibaba Cloud:-

&#x20;  --------------

A major player in Asia, offering competitive cloud services globally.



4\. IBM Cloud :-

&#x20;  ---------

Focuses on hybrid cloud and AI-driven solutions for businesses.



5\. Oracle Cloud :-

&#x20;  ------------

Focuses on enterprise applications and databases.

Each of these vendors offers a range of services, but AWS remains the most popular due to its vast infrastructure and support for businesses of all sizes.



How Companies Are Using the Cloud

* Netflix runs its entire platform on AWS so it can scale globally, stay online during peak demand, and stream content reliably to millions of users at once.
* Spotify uses the cloud to handle millions of songs and users, scaling quickly when new music or features are released.
* Instagram relies on the cloud to store massive amounts of photos and videos and deliver them fast to users around the world.
* Online stores use the cloud to handle traffic spikes during black friday without buying permanent infrastructure.
* These companies use the cloud because it lets them scale easily, reduce costs, stay reliable, and focus on improving their products instead of managing hardware.



Next, you’ll apply these same ideas by deploying your cyber security training app in a simulated cloud environment!



Answer the questions below :

What is the characteristic of cloud environments that enables you to handle an unexpected increase in access to your application?



Answer : Scalability (or Rapid Elasticity)



What is the most common type of cloud deployment used?



Answer : Public Cloud



Suppose you want to deploy an application to the internet, focusing only on application development and leaving infrastructure to others. What type of cloud service is the best?



Answer : PaaS

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 Lab :-

\----------

Deploying a Cloud Instance :-

\---------------------------

So far, you’ve learned what cloud computing is and why companies use it. Now it’s time to see those ideas in action by deploying a cloud environment to launch your cyber security app training!

In this exercise, you’ll use a cloud interface similar to the AWS platform. The goal is not to memorize buttons, but to understand how cloud resources are easily created and managed in a real-world scenario.



Open the Cloud Console site by clicking the View Site button below, and let's create your cloud environment!



Basic Cloud Terminology

To complete this exercise, you only need to understand a few basic concepts from AWS:



1. EC2 (Virtual Computer / Server) :-

&#x20;  -------------------------------

EC2 represents a virtual computer in the cloud. Just like a real computer, it has a CPU and memory (RAM) and can run applications. Whenever you add an EC2 instance, you are adding a computer to your environment.

2\. Instance Type (for example: t2, t3, m5) :-

&#x20;  ---------------------------------------

Instance types describe how powerful the virtual computer is. Some have more CPU and RAM and are therefore more expensive. You choose the Instance Type based on your needs, knowing that:



Bigger instances = more power + higher cost

Minor instances = less power + lower cost



Step-1 :-

\------

First we click on the visit site button.

Step-2 :-

\------

Now, we go to the Create Lab Machine block on the right side of the page to create the lab machines for our application.

Step-3 :-

\------

Now create our application interface machine by click on create virtual machine. Set the following configuration:



Instance Name: application-interface

Instance Type: t3.micro

Status: running

Then click on create VM button.

Step-4 :-

\------

Now same way  create two testing computers for users to practice their cyber security skills.

Since these are test machines, let's use a more powerful instance type: m5.large with the following configuration :



Machine 1:

\---------

Instance Name: study-machine-1

Instance Type: m5.large

Status: running



Machine 2:

\---------

Instance Name: study-machine-2

Instance Type: m5.large

Status: running

same way click on create VM.

Step-5 :-

\------

Now scroll down and we see the billing of our machines monthly cost.

Step-6 :-

\-------

Now we go Instances where machines or VM's name, type, status, cost, and action we see here under active we click on stop button of study-machine-1 and study-machine-2 to stop them.

Step-7 :-

\------

Now if we see billing then can see now the monthly cost is changed to 170 to 30 credits.

Answer the questions below :

What is the total cost of credits of the entire environment if study-machine-1 and study-machine-2  are stopped?



Answer : 30

\------



How many credits does an m5.large EC2 instance cost per month?



Answer : 70

\------

What is the total cost of credits if only the new instances we created are running?



Answer : 150

\------



What would be the total running cost of the entire environment you created if you add a third t3a.small study machine?



Answer : 188

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\------

Conclusion :-

\-----------

In this room, you explored the core ideas behind cloud computing and how it enables flexible, scalable, and cost-effective access to computing resources.



Key Terminology :-

\----------------

Let's quickly review some concepts we learned in this room:



* Public Cloud :-

&#x20;  ------------

Cloud services you access over the internet that many people and companies share.

* Private Cloud :-

&#x20;  --------------

A cloud built just for one company, so they have more control and security.

* Hybrid Cloud :-

&#x20;  -------------

A mix of public and private clouds that can work together and share data.

* IaaS :-

&#x20;  -----

A service where you rent basic computer parts like servers and storage from the cloud.

* PaaS :-

&#x20;  -----



A service that gives you a ready-to-use environment to build and run apps without managing servers.

* SaaS :-

&#x20;  -----

Software you use online without installing anything, like Gmail or Zoom.

* EC2 :-

&#x20;  ----

Amazon’s cloud computers that you can quickly create, use, and resize whenever you need them.



We also concluded that the key benefits of cloud computing are:



* Scalability
* On-demand self-service
* Pay only for what you use
* Security
* High availability
* Global access

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



Operating Systems Introduction Room :-

\------------------------------------

Task 1 :-

\-------

Introduction :-

\------------

You turn on your phone or laptop every day, and everything just works: apps launch, files open, music plays, and the whole system feels seamless. But what actually makes all this possible? In the Computer Fundamentals module, you explored the physical components of a computer and the different types of computing devices. Now it’s time to uncover the invisible layer that ties it all together: the operating system, or OS.



A graphic of an airport scene representing the various components of a user's computer.



Scenario :-

\---------

Your friend just upgraded their primary computer and, knowing you're getting into tech, has generously gifted you their old machine. It's been sitting untouched for a while, and he can't remember much about it, only that it “used to run well”. Before you can decide whether to upgrade it, wipe it, sell it, or turn it into your next project, you need to figure out precisely what you're dealing with.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------Task 2 :-

\-------

The Invisible Manager :-

\----------------------

An operating system (OS) is the core software that coordinates everything happening on a computer. It sits between the user, applications, and the system’s physical hardware, acting as the invisible manager that keeps the entire machine running as one unified system.



A visual diagram illustrating the layers of a computer with the physical hardware on the bottom, operating system second, the applications third, and the user on top.



A helpful analogy is to think of your computer as a busy airport, with all its components functioning together.



Your hardware (CPU, RAM, storage, connected devices): The runways, airplanes, fuel systems, radar, and other physical infrastructure.

Your applications (web browser, game launcher): The various airlines and their passengers, all trying to take off, land, and request services.

Your operating system (Windows, Linux, macOS): The entire air traffic control system, directing all of this activity. It schedules resources, manages traffic, resolves conflicts, and ensures safety.

A graphic showing an airport from the perspective of air traffic control which represents the computer's operating system.



We need an operating system because it provides this all-important job of coordination and structuring that makes modern computing possible. Without an OS, each application would need direct control over the CPU, memory, files, devices, and security. This would quickly cause conflicts, and the OS handles this by acting as the central organizer. In the Computer Fundamentals module (coming soon), you learned about various computer components and their duties. Now, we will see how the operating system manages and allocates these resources when you use your PC.



System Privilege Layers :-

\------------------------

Inside a modern computer, different parts of the system operate at various permission levels. Some components can communicate directly with the hardware, while regular applications run in a safer, restricted environment. This separation is intentional and helps prevent conflicts and security issues.



1. Kernel space :-

&#x20;  -------------

The privileged, locked-down core of the OS. This is where the kernel, the part of the operating system that directly manages hardware and system resources, runs. It has unrestricted access to the CPU, memory, storage, and all hardware components.



2\. User space :-

&#x20;  ----------

Where all standard applications run. Applications in the user space are deliberately prevented from accessing hardware directly. Whenever they need to open or save a file, play a sound, or connect to Wi-Fi, they must make a system call and request that the kernel act on their behalf.

Building on our airport analogy, let's zoom in on the concept of privilege separation. The kernel space is the control tower, a strictly secured area where only trusted air-traffic controllers (the kernel) work. They alone can directly control the runways, radar, and other hardware. Applications in the user space are like airlines and passengers on the ground. They can't enter the tower or touch the equipment. Instead, they radio requests (system calls) to the tower, which handles them safely. This separation keeps the OS reliable: one faulty app can't crash the whole system, just as no airline can operate safely without the tower's control.



Operating System Duties :-

\-----------------------

Now that you know what an operating system is and how system privilege is separated, let’s look at what it actually does behind the scenes. Every OS is responsible for a few core duties that allow your computer to run safely, efficiently, and predictably.



|OS Responsibility|What the OS Does|Example|
|-|-|-|
|Process Management|Creates, schedules, prioritizes, and terminates running programs. The OS decides how much CPU time each process gets, making multitasking feel seamless|Opening multiple apps, like your browser, music player, and social media, without your computer freezing|
|Memory Management|Allocates RAM to processes, protects the app's memory from other processes, and reclaims memory when apps are closed. When RAM runs low, the OS uses virtual memory to keep your system stable|Opening multiple app at once, the OS allocates RAM to each one and keeps them isolated so they don’t interfere or crash each other|
|File System Management|Organizes files into directories, handles naming, paths, permissions, metadata (name, size, type, timestamps)|Creating a new folder, saving a photo, or setting a file to "read only"|
|User Management|Handles multiple user accounts, authentication, and permissions to determine who can access what|Logging in with your password and keeping your files inaccessible to other user accounts|
|Device Management|Loads drivers and provides a universal interface (hardware abstraction layer), so apps can say “print this” or “play this sound”|Plugging in a new mouse, printer, or external hard drive and having it work immediately<br />|



Operating System Security :-

\-------------------------

It is important to understand that every OS also acts as a security foundation. Before any antivirus, firewall, or security tool is introduced, the OS is already enforcing protections in the background, some of which we covered above.



At a basic level, your operating system handles



* Authentication :-

&#x20;  ---------------

Verifies who you are through login passwords and biometrics

* Permissions :-

&#x20;  ------------

Controls exactly what each user and app is allowed to read, write, or execute

* Isolation :-

&#x20;  ----------

Keeps every process in its own protected box (kernel/user space separation)

* System Protection :-

&#x20;  -----------------

Safeguards critical system files and settings from unauthorized changes



Lab :-

\----

Step-1 :-

\-------

First we go to About this Computer by click on this.

Step-2 :-

\-------

Now we see 4 tabs those are system, process, Resources, File systems. In system see information about kernel, os name with the 64 bit or 32 bit specification and hardware level information like Memory, processor , graphics, and in system status see the available storage. In processes show what process are run. In Resources we see current information about CPU History (CPU utilization) and next see Memory and swap history where how my memory used show and also the swap space and next we see Network history where how much data transmit and received show. Atlast we see File systems where we see the storage point and it is what type of file system.



Answer the questions below:

Which OS space has unrestricted access to your computer's hardware?



Answer: Kernel Space

\------

Which OS responsibility manages user accounts, authentication, and permissions?



Answer : User Management

\------

After opening the About This Computer shortcut, you are greeted with an overview of the system's specifications.

What version of Ubuntu Mate is your computer running?



Answer : 1.26.2

\------

Check out the Hardware section of the System tab.

How much memory is allocated to your machine?



Answer : 1.9 GIB

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

OS Interaction and Landscape :-

\-----------------------------

OS Interfaces :-

\--------------

Now that you have a solid understanding of the operating system and its various responsibilities, let's look at how we interact with the OS. Interaction with the OS can be divided into two main parts: the graphical user interface (GUI) and the command-line interface (CLI).



1. Graphical User Interface :-

&#x20;  ------------------------



The GUI is what you're most likely used to interacting with. It provides a graphical representation of all the information you want to access on your computer. Think of folder icons, windows for your applications, and menus for settings. We can imagine the analogy of using a navigation application. You tap an icon of the place you want to visit, and the app generates directions for you, eliminating the need for typing.



2\. Command-line Interface :-

&#x20;  ----------------------



The CLI is where you enter specific text-based commands to retrieve or manipulate information. Instead of clicking on icons, you tell the computer exactly what you want using words and syntax that the system understands. This gives you far more precision, control, and speed, especially for advanced tasks, but it requires familiarity with the commands. Back to the maps analogy. Using the CLI is like entering the exact GPS coordinates of your destination. It’s direct and extremely accurate, but only if you know the correct information to type.



Later in this module, you will explore the CLI on both Linux and Windows to learn how to navigate files, inspect system information, and interact with your OS beyond the GUI.



In the screenshot below, you can see that the GUI and CLI are both used to retrieve the same information. In this case, to display the contents of the ubuntu user's home directory. The GUI requires a few clicks for folder navigation, whereas the CLI requires a command to list the directory contents.



A composite screenshot of the ubuntu user's home directory listing the directory contents using file explorer (GUI) on the left and command-line (CLI) on the right.



The Operating System Landscape :-

\------------------------------

Nice! We are gaining a much clearer picture of the OS, its responsibilities, and how we can interact with it to manage our computer. Now it's time to look at the bigger picture; not all operating systems are the same. Different devices and jobs demand different designs, ranging from your phone to a web server in a data center. Below are the five major categories you'll run into in the real world:



|Operating System Type|Primary Use Case|Key Characteristics|
|-|-|-|
|Desktop|Personal computers, daily work, gaming, content creation|Rich graphic interface, runs many apps at once, user-focused|
|Server|Web hosting, databases, cloud services, back-end|Headless (no GUI), maximum uptime, multi-user, remote access|
|Mobile|Smartphones and tablets|Touch-based UI, power efficient, always connected, app sandboxing|
|Embedded|Appliances, cars, IoT devices, smart TVs, routers|Tiny footprint, runs on limited hardware|
|Virtual/Cloud|Lab machines, containers, cloud instances|Lightweight, scalable, rapid deployment|



Real World Operating Systems :-

\----------------------------

Now that you’ve seen the different types of operating systems and what they’re designed for, let’s look at the major families of operating systems you’ll encounter in the real world. Each family fills one or more of the OS types we just explored. To keep things organized, we’ll highlight the common versions or distributions you’ll see in each and follow the same categories as above: Desktop, Server, Mobile, Embedded, and Virtual/Cloud.



Desktop :-

\-------



1. Windows :-

&#x20;  --------

The most widely used operating system on personal computers

Windows 10 (end-of-life), Windows 11



2\. macOS :-

&#x20;  ------

Apple's desktop OS, known for its polished GUI and integration with other Apple devices

Sonoma (14), Sequoia (15), Tahoe (26)



3\. Linux :-

&#x20;  ------

Not a single OS but a family of open-source operating systems called distributions

Ubuntu, Debian, Fedora



Server :-

\-------



1. Windows :-

&#x20;  --------

Used in large networks, data centers, and corporate environments

Server 2016, 2019, 2022, 2025



2\. Linux :-

&#x20;  ------

The vast majority of web servers, trusted for its reliability and open-source nature

Ubuntu Server, Debian, CentOS, Red Hat



3\. Unix :-

&#x20; ------

Large enterprises, finance, telecom, government

IBM AIX, Oracle Solaris



Mobile :-

\-------



1. Android :-

&#x20;  --------

The most widely used mobile OS, which runs on phones, tablets, and smart devices

Android 14 - 16, Manufacturer versions



2\. iOS :-

&#x20;  ----

Apple's mobile OS running on iPhones, iPads, and other devices

iOS 17, 18, 26



Embedded and IoT Devices :-

\------------------------



1. Embedded Linux :-

&#x20;  ---------------

Specialized OS built into devices with dedicated functions

OpenWrt, Ubuntu Core, Yocto Project



2\. Real-Time OS :-

&#x20;  -------------

Designed for apps where tasks need guaranteed response times (aircraft controls)

FreeRTOS, VxWorks, QNX



Virtual and Cloud :-

\-----------------



1. Cloud/VM :-

&#x20;  ---------

Massive data centers that host websites, apps, and streaming services

Ubuntu LTS, Amazon Linux, Rocky Linux



2\. Container-optimized :-

&#x20;  -------------------

Lightweight alternatives to VMs that package just the app and its dependencies

Alpine Linux, Bottlerocket AWS, Flatcar Linux

A composite image of the Windows logo, Tux Linux logo, Apple logo, and Android logo to represent different operating systems discussed.



Why So Many Operating Systems?

Different devices and environments require different capabilities from an OS. A laptop must be user-friendly and support multitasking. Servers require stability, security, and must be able to run continuously without interruption. Mobile devices need power efficiency and hardware integration to extend battery life. Embedded systems use lightweight operating systems designed for a specialized purpose.



The companies and communities that develop these operating systems also have their own goals. Some focus on ease of use, performance, security, openness, or customization. Because each environment values different capabilities, no single OS is the perfect fit for every situation. Instead, an ecosystem of operating systems has evolved.



Continuing Your Investigation :-

\------------------------------

From the previous task, you learned that your new computer is running the Ubuntu distribution of Linux. You were also able to determine the version and release. Let's continue the investigation and gather further information about the system. You will continue to use the About This Computer shortcut, then jump into the Home directory, which can be found on your computer's Desktop.



A graphical representation of a computer home screen displaying a home icon, folder icon, and open browser with a magnifying glass overlaying it to represent the investigation portion of the task.



Step-1 :-

\------

Here first go about this computer and then go File systems and there see the mount point is /dev/root and it file system is ext4. (here get first question answer)



Step-2 :-

\-------

Now we go to terminal then give command ls there see hoe directory so we give command cd /home now we go to home directory and there see three directory (alex, guest, ubuntu) thats how we see three directory and get 2nd question answer.



Step-3 :-

\------

now give command cd /home and go home directory and next to go the alex directory again give cd /alex and there see note.txt file to see inside it we give command cat note.txt and we get the flag THM{new\_pc\_for\_free!} and that's way our third question answer we get.

* 

Answer the questions below:

1. Open the File Systems tab in System Monitor.

What Type is listed for the /dev/root device?



Answer : ext4



2\. After opening the Home directory on the Desktop, how many user directories exist?



Answer : 3



3\. Navigate to Alex's home directory and explore the Documents folder.

What is the flag value contained in note.txt?



Answer : THM{new\_pc\_for\_free!}

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conclusion :-

\----------

Well done, you've reached the end of Operating Systems Introduction. In this room, you learned what an OS really does behind the scenes and explored key concepts, including privileges, user management, memory handling, and processes. In the practical exercise, you investigated a mystery computer gifted to you by a friend. You used the operating system to take a peek into the hardware and file systems it helps manage.



Key Terminology :-

\----------------

Let’s recap the core terms you’ve learned. These definitions will help solidify your understanding before moving on to further learning.



* Operating system (OS) :-

&#x20;  ----------------------

The core software that manages hardware, applications, and all system resources.



* Kernel space :-

&#x20;  -------------

The OS’s highly privileged area with direct hardware access, and the home of the kernel, which directly manages hardware and system resources.



* User space :-

&#x20;  -----------

The area where regular applications run with limited permissions for safety and system stability.



* Graphical user interface (GUI) :-

&#x20;  ------------------------------

The visual part of the OS, windows, icons, and menus, that lets you interact through clicking and tapping.



* Command-line interface (CLI) :-

&#x20;  -----------------------------

A text-based interface where you type commands to control the system with precision and speed.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Windows Basics Room :-

\-------------------

Task 1 :-

\-------

Introduction :-

\-------------

Every operating system has its own personality, and if you’ve used a computer at school, work, or home, there’s a good chance you’ve already met the most familiar one: Microsoft Windows. In the previous room, you explored what an operating system is, the behind-the-scenes manager that keeps your device running smoothly. Now it’s time to step into a real example and see the previously learned concepts take shape on a system you may already recognize. In this room, you’ll get hands-on experience with the Windows interface and begin building practical skills that will lay the foundation for the subsequent rooms of the module.



Scenario :-

\--------

In this room, you’ll take on the role of a new employee starting your first day at TryHatMe. Once you log in to your workstation, you’ll get to know the Windows desktop, learn how the interface works, open tools from the Start menu, and find your way through company folders. Your supervisor will guide you in creating and organizing files, changing system settings, checking the Task Manager, and reviewing basic security settings. By the end of these onboarding tasks, you should feel comfortable using Windows and handling the daily tasks you'll be expected to handle.



A graphical illustration of a worker running the assembly line at the fictional company TryHatMe.



Learning Objectives :-

\-------------------

Navigate the Windows graphical interface, including the desktop, taskbar, and Start menu

Use File Explorer to browse folders, understand file paths, and organize files effectively

Check system settings and personalize the Windows environment using the Settings app

Use basic system tools like Task Manager and Windows Security to monitor performance and verify system protection

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

Exploring the Windows Workspace :-

\--------------------------------

Before Windows had its current polished look, Microsoft’s operating systems were much simpler. Early computers ran MS-DOS, which showed a black screen where you had to type commands instead of clicking icons. In 1985, Microsoft released Windows 1.0, a basic graphical user interface (GUI) built on top of DOS, introducing windows, menus, and mouse controls to personal computers. Over time, Windows has added more features, which turned the original shell into a complete operating system. Today, the modern Windows OS is the result of those changes. Let’s dive into Windows and see how the operating system concepts you learned about in the previous room present themselves in the world’s most widely used desktop operating system.



A composite screenshot showing the evolution of the Windows OS with Windows 1.0 on the left, Windows Me in the center, and Windows 11 on the right.



* Logging in and Authentication :-

&#x20;  ------------------------------

Before gaining access to the Windows Desktop, you must authenticate (prove your identity) to the system. The authentication process verifies your identity and determines the actions you're allowed to take once logged in. When a Windows system starts, it displays a login screen where a user account must be selected and authenticated with a password, PIN, or another verification method. Each user is assigned a set of permission levels that determine their access to files, settings, and system functionality. Windows commonly uses the account types below.



* Guest :-

&#x20;  ------

A restricted account intended for temporary access, with minimal permissions and no ability to change system settings

Standard: A user account for everyday tasks, such as running applications and changing personal settings, without access to system-wide changes

Administrator: A privileged account with full control over the system, including software installation, configuration changes, and user management

A screenshot of the Windows Server 2019 login screen showing the Administrator username and blank password.



Upon starting up the machine in the previous task, you are automatically logged in using an Administrator account. This will allow you to explore system settings, install programs, and perform administrative actions without being restricted by permission limitations.



* The Windows Desktop :-

&#x20;  --------------------

In the last room of this module, we explored the comparison of an OS to an airport. Let's continue with this analogy. If you, the user, are a passenger, and the login screen represents the airport security checkpoint, you can consider the Desktop to be the airport terminal. After entering, it is the first area you gain access to, and all other subsequent areas branch out from this point.



A graphical illustration of an airport terminal representing the computer desktop.



Let's have a look at the Windows Desktop and cover some of its core features together. When you first log in, you're presented with two main areas.



* Desktop :-

&#x20;  --------

The main workspace where files, folders, and shortcuts live



* Taskbar :-

&#x20;  --------

A control strip that provides access to applications, system tools, settings, and notifications

Let's break these down further to get a better picture. Please note that the instance used in this room and the screenshot below are using Windows Server 2019. While newer Windows versions may differ slightly, these core components and concepts remain consistent.



1. Desktop icons :-

&#x20;  --------------

Shortcuts to items like the Recycle Bin, folders, and frequently used applications. It is fully customizable



2\. Start menu :-

&#x20;  -----------

Primary way to access applications, settings, and power options. From here, you can log out, restart, or power off your machine



3\. Search :-

&#x20;  ------

Quickly find applications, files, folders, and system settings by using keywords



4\. Task View :-

&#x20;  ----------

Allows you to see all currently open windows and quickly switch between them



5\. Pinned Applications and Folders :-

&#x20;  -------------------------------

Your most used applications and folders can be pinned here



6\. Network and Audio settings :-

&#x20;  --------------------------

This section can be customized to suit your needs



7\. Date and Time :-

&#x20;  --------------

Opens up to a full calendar. Date and time settings can be accessed here, too



8\. Notifications :-

&#x20;  -------------

Displays computer or application notifications. Network and other settings can also be accessed A screenshot of the Windows desktop highlighting the desktop icons, start menu, search, task view, pinned apps and folders, network and audio settings, date and time, and notifications.



* Start Menu :-

&#x20;   ----------



When using Windows, the Start menu can be accessed by clicking the Windows icon located at the bottom left of the taskbar. If we consider the Windows Desktop to be an airport terminal, the Start menu is the departure board or information desk. It is the area where we see what is available: apps, files, folders, settings, and power options. You can think of it as a quick-access menu.



A screenshot of the Windows Start menu highlighting the different options it provides, including user options, documents, pictures, settings, and power, as well as quickly accessible apps, settings, and folders.



* Built-in Tools and Apps :-

&#x20;  ------------------------

Windows ships with many useful built-in tools and applications that you will use daily. Beyond the wide range of settings available to manage your system, Windows also includes simple but powerful tools such as Notepad for editing text files and File Explorer for navigating and managing files. These tools are available immediately and form the foundation of everyday Windows usage. All of them can be accessed via the Start menu and search bar. The built-in tools on Windows are like airport services and amenities, the things already available in the terminal to help you get tasks done.



A composite screenshot of the Windows built-in applications, including the calculator, file explorer, notepad, and paint.



* Getting System Information :-

&#x20;  ---------------------------

Windows includes a built-in Settings application that allows you to configure and view information about your system. To get to know your new work PC better, we’ll start by investigating the machine we’re working with. Within the Settings app, there's a helpful section called About your PC, that provides key details about the system. A shortcut to About your PC has been created on the Desktop. Open it now. Alternatively, you can practice using the Start Menu or Search feature to locate it.



The About your PC page provides an overview of security, device, and operating system information. We’ll use this information to become familiar with our environment and begin answering the first questions in this task.



A composite screenshot of the About your PC Windows application desktop shortcut and the main page of the application displaying security, device, and operating system details.



* File Exploration and Management :-

&#x20;  -------------------------------

Great, now we have an understanding of the system we are working with. Let’s take a look at how Windows handles file exploration and management as we access some of the onboarding documents for your new position. Before we dive into using File Explorer, let’s quickly cover how Windows organizes files and directories. Windows uses a hierarchical folder structure, meaning folders can contain other folders and files inside them. This structure helps keep data organized and makes it easier to locate information as systems grow larger. Common locations, such as the Desktop, Documents, and Downloads, serve as primary directories for storing files. Within these locations, subfolders are used to group related files together. Understanding this layout will make navigating the system and managing files much easier.



Lab :-

\----

Step-1 :-

\-------

First we click on the TryHatMe Onboarding folder in our desktop.

Step-2 :-

\-------

Clicking the folder name will show us the full path to the chosen folder

C:\\Users\\Administrator\\Desktop\\TryHatMe Onboarding

Step-3 :-

\-------

Now go About your pc.Now in about sections we see various information such as Device Name, Processor, Installed Ram, Device ID, Product ID, System Type.

Step-4 :-

\-------

Now we see the first questions answer that Device name we see device name given is TryHatMe.

Step-5 :-

\------

we see the installed Ram is also given is 4.00 GB that is our 2nd question answer.

Step-6 :-

\------

Now we scroll down and see Windows Specification and under it also various information given such as Edition, Version, Installed on and Build OS. There we see third question answer that the version is 1809.

Step-7 :-

\------

Now to Find the final forth question answer we go TryHatMe onboarding and click on it and then we see welcome.txt we click on it and open it and there we see that flag is given  THM{welcome\_to\_tryhatme!} that's how our final question is also solve.



Answer the questions below:

1. Please ensure the lab machine is open in split-screen, then take a look at the computer's Desktop.

After opening About your PC, navigate to the Device specifications section.

What is the Device name specified?



Answer : TryHatMe

\-------



2\. Continue looking through the Device specifications.

How much RAM is installed on your new work PC?



Answer : 4.00 GB

\-------



3\. Scroll down to the Windows specifications section.

Which Version of Windows Server 2019 Datacenter is installed?



Answer : 1809

\------



4\. Explore the TryHatMe Onboarding folder located on your computer's Desktop.

What is the flag value found within Welcome.txt?



Answer : THM{welcome\_to\_tryhatme!}

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Configuring and Securing Windows :-

\---------------------------------

Applications are the programs and tools you use to perform tasks on your computer, from browsing the web and editing photos to managing settings on your PC. We already discussed a few of the built-in applications Windows provides, but knowing how to install, update, and remove applications is a core skill for everyday Windows use. Let's briefly revisit the airport analogy to gain a better understanding of this concept. Updating your OS or apps is like changing flights or reserving a seat. Installing a new app is comparable to scheduling a new flight, and removing apps is like canceling a booking you no longer need. These three processes enable you to make the necessary changes to your system, ensuring you have exactly what you need and that your system remains secure.



Updating Your Applications :-

\--------------------------

Keeping your operating system and applications up to date is an important part of maintaining a secure and stable system. Updates will often include security patches, performance updates, and bug fixes.



Windows Updates :-

\---------------



Windows includes a built-in update tool called Windows Update, which keeps the OS and some native applications and security features up to date. Windows Update can be accessed through the Settings app and may install updates automatically, depending on your configuration.



A composite screenshot of Check for updates in System settings with the Windows Update page in Settings showing the current available updates.



Updating Applications :-

\---------------------



Application updates work differently depending on how the software is installed.



* Built-in applications may update automatically in the background
* Third-party applications often include their own update mechanisms
* Some applications will prompt you to update upon launch
* Some require you to check for updates or download a new installer manually



1. Installing Applications :-

&#x20;  -----------------------

Now that you've seen how updates work within the Windows OS and for applications, let's take a look at installing new ones.



2\. Microsoft Store :-

&#x20;  ---------------

Provides a curated and safe option for installing apps to Windows, although it is not available by default on Windows Server.



3\. From the Internet :-

&#x20;  -----------------

In many environments, apps are installed by downloading an installer directly from a trusted vendor's website. They usually come in an .exe or .msi file and guide the user through the



4\. installation process :-

&#x20;  ---------------------

A composite screenshot of the Microsoft Store application and Windows download page for 7-Zip.



Task 1: Hands-On Application Installation :-

\-----------------------------------------



Action (How to do) :-

\------------------



1. Double-click the TryHatMe Onboarding folder on your Desktop.



2\. Double-click the TryHatMeWelcome installer file.



3\. Click through the setup wizard options to complete installation.



4\. What You See: The installer window opens, guiding you through the steps and providing the information required for the task question.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2: Application Uninstallation Methods :-

\------------------------------------------



Action (How to do) :-

\-------------------

Practice navigating the four uninstallation methods :-

\---------------------------------------------------



* Microsoft Store :-

&#x20;  ----------------

Open Store → Library / Installed Apps → Click ... next to the app → Uninstall.



* Windows Settings :-

&#x20;  -----------------

Open Settings → Apps → Installed apps → Click ... → Uninstall.



* Control Panel :-

&#x20;  --------------

Open Control Panel → Programs → Uninstall a program → Right-click the app → Uninstall.



* Built-in Uninstaller :-

&#x20;  ---------------------

Navigate to the app's directory in C:\\Program Files → Run uninstall.exe.



What we See :-

\------------

Different administrative layouts for viewing installed software, system storage usage, and removal tools

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3: Navigating System Settings :-

\-----------------------------------



Action (How to do) :-

\-------------------

Open both configuration applications using the Desktop shortcuts:



* Windows Settings :-

&#x20;  ------------------

Access modern configuration options (Display, Accounts, Network, Security).



* Control Panel :-

&#x20;  --------------

Access legacy management options (Administrative Tools, Power Options, User Accounts).



What You See :-

\-------------

Settings displays a unified, modern interface, while Control Panel shows classic applet icons for advanced system tweaks.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4: System Monitoring via Task Manager :-

\-------------------------------------------



Action (How to do) :-

\-------------------

Double-click the Task Manager shortcut on your Desktop.



What we See (Tab Breakdown):



* Processes :-

&#x20;  ----------

Active applications, background processes, and live CPU/RAM resource usage.



* Performance :-

&#x20;  ------------

Real-time hardware performance graphs (CPU, Memory, Disk, Network).



* Users :-

&#x20;  ------

Logged-in user accounts and resource consumption per user.



* Details :-

&#x20;  --------

Advanced technical process data, including Process IDs (PIDs).



* Services :-

&#x20;  ---------

System background services and their execution status (Running or Stopped).

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5: Custom Virus \& Threat Protection Scan :-

\---------------------------------------------



Action (How to do) :-

\------------------

&#x20;

* Open Windows Security using the Desktop shortcut or Start menu.



* Select Virus \& threat protection.



* Click Scan options under Current threats.



* Select Custom scan, then click Scan now.



* Select the TryHatMe Onboarding folder on your Desktop as the target.



* Click See details on the scan results screen once finished.



What You See :-

\------------

Detection of a harmless test file along with its severity level and path details to answer the final task question.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 6: Windows Defender Firewall Overview :-

\-------------------------------------------



Action (How to do) :-

\------------------

Open Windows Defender Firewall and click Advanced settings.



What You See :-

\-------------



1. Profiles :-

&#x20;  ---------

Active profile status for Domain (enterprise), Private (home/lab), and Public (untrusted networks).



2\. Advanced Rules :-

&#x20; ---------------

Inbound and Outbound rule lists showing allowed/blocked traffic, protocols, and ports.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Lab :-

\----

Step-1 :-

\------

Click on TryhatMe and write click on the TryHatMe welcome application and install in c drive program file X86 and there we set up the TryHatMe Onboarding folder and then open that folder and click on the welcome application and then our first question flag is popup which is THM{your\_first\_day!} that's how our first question is solved.

Step-2 :-

\-------

here we follow this steps settings ---> Time \& Languages ---> Region ---> Here see our Region is give united states. That's how we get second question answer.

Step-3 :-

\-------

Now we follow this steps open Task manager ---> Go on users tab ---> Now see Administrator ( this is current logged in user) that's how we solve the third question answer.

Step-4 :-

\-------

now we follow this steps go search ---> run ---> give this in run Virus:DOS/EICAR\_Test\_File  ---> ok ---> our that malicious file is quarantined then click on see details ---> in first path in Affected items: we get file: C:\\Users\\Administrator\\Desktop\\TryHatMe Onboarding\\NewHireDocs\\tryhatmemaldoc.txt so here the final answer or file name we submit is tryhatmemaldoc.txt. This will be the final answer of forth question.



Answer the questions below:

1. Use the TryHatMeWelcome installer located within the TryHatMe Onboarding folder.

What is the flag value you receive after installing and running the application?



Answer : THM{your\_first\_day!}



2\. Investigate the Time \& Language section of the Windows Settings app.

Which country or region is your computer currently set to?



Answer : United States



3\. Open the Task Manager on your workstation's Desktop and navigate to the Users tab.

Which account is currently logged in?



Answer : Administrator



4\. After performing your custom scan, click Virus:DOS/EICAR\_Test\_File and select See details.

What is the file name shown in the Affected items section?



Answer : tryhatmemaldoc.txt



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conclusion :-

\-----------

Nicely done! You’ve reached the end of Windows Basics. In this room, you explored the fundamentals of the Windows operating system. You navigated the Windows interface, examined system properties, learned about application management, worked with files and folders, and managed security settings that make up a Windows environment.



Through a hands-on lab, you completed your first day at TryHatMe, using the Windows Server 2019 operating system to read files, install programs, and run security scans on your new workstation. These skills form the foundation for both general system usage and deeper technical understanding later on in your learning and professional journey.



Key Terminology :-

\----------------

Let’s recap the core terminology and applications you’ve learned about in this room. These definitions will help solidify your understanding before moving on to further learning.



1. Desktop :-

&#x20;  --------

The main workspace where files, folders, and shortcuts live



2\. Taskbar :-

&#x20;  --------

A control strip that provides access to applications, tools, settings, and notifications



3\. Start Menu :-

&#x20;  -----------

The primary way to access applications, settings, and power options, signified by the Windows logo



4\. Search :-

&#x20;  -------

A quick access method of locating applications, settings, and files by entering search terms



5\. File Explorer :-

&#x20;  -------------

The built-in Windows tool to browse, manage, and organize files and folders



6\. Windows Update :-

&#x20;  ---------------

A built-in update tool that helps keep your OS, native apps, and security features up to date



7\. Microsoft Store :-

&#x20;  ---------------

The native Windows application for installing trusted applications



8\. Windows Settings :-

&#x20;  ----------------

A centralized location for configuring system, device, personalization, and security settings



9\. Control Panel :-

&#x20;  --------------

The legacy management interface that provides access to system configuration options



10\. Task Manager :-

&#x20;   -------------

A Windows tool for monitoring what is happening on your system in real time



11\. Windows Security :-

&#x20;   -----------------

The central dashboard for managing Windows built-in security tools



12\. Windows Defender Firewall :-

&#x20;   -------------------------

The firewall designed to help protect your system from unauthorized network traffic

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Linux CLI Basics Room :-

\----------------------

Task 1 :-

\-------

Introduction :-

\------------

In cyber security, Linux is everywhere, powering servers, security tools, and even hacking environments. However, before you can defend systems or investigate incidents, you need to know how to navigate the Linux OS using the command-line interface (CLI). This room takes you on a guided mission as a brand-new intern in a cyber security team. We will explore the absolute basics of Linux CLI through hands-on tasks, simple missions, and beginner-friendly explanations.



Answer the questions below:

What does "CLI" stand for?

Answer : Command-line interface

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Navigation Mission: "Find the Missing Notes" :-

\---------------------------------------------

Step-1 ("Where Am I?") :-

\-----------------------

When you first open a terminal, you might not know what part of the system you're in.

Use this command to find out: pwd





PWD Command

ubuntu@tryhackme:\~$ pwd

/home/ubuntu

It stands for "print working directory", which basically means "show me the folder I'm currently in".



Step-2 ("What's Around Me?") :-

\-----------------------------

Now that you know where you are, let's see what files and folders are here: ls





ls Command

ubuntu@tryhackme:\~$ ls

Desktop    Downloads  Pictures  Templates  logs

Documents  Music      Public    Videos     projects

This lists the content of the current directory. If we need more details, we can try: ls -l





ls -l Command

ubuntu

@tryhackme:\~$ ls -l

total 44

drwxr-xr-x 2 ubuntu ubuntu 4096 Feb 27  2022 Desktop

drwxr-xr-x 6 ubuntu ubuntu 4096 Dec 11 12:45 Documents

drwxr-xr-x 2 ubuntu ubuntu 4096 Feb 16  2024 Downloads

drwxr-xr-x 2 ubuntu ubuntu 4096 Feb 27  2022 Music

drwxr-xr-x 2 ubuntu ubuntu 4096 Feb 27  2022 Pictures

drwxr-xr-x 2 ubuntu ubuntu 4096 Feb 27  2022 Public

drwxr-xr-x 2 ubuntu ubuntu 4096 Feb 27  2022 Templates

drwxr-xr-x 2 ubuntu ubuntu 4096 Feb 27  2022 Videos

drwxr-xr-x 4 ubuntu ubuntu 4096 Dec 11 12:29 logs

drwxr-xr-x 5 ubuntu ubuntu 4096 Dec 11 12:29 projects

drwx------ 3 ubuntu ubuntu 4096 Sep 12  2024 snap

The output displays important information about the files and directories like file sizes, permissions, dates, and more.



Hidden Files



In order to get the hidden files in the directory, we can append the command to ls -al, and it will display all the hidden files present in the directory, as shown below:





ls -al Command

ubuntu@tryhackme:\~$ ls -al

total 144

drwxr-xr-x 24 ubuntu ubuntu  4096 Feb 10 10:48 .

drwxr-xr-x  3 root   root    4096 Feb 10 10:36 ..

\-rw-------  1 ubuntu ubuntu   439 Feb 10 06:47 .Xauthority

\-rw-rw-r--  1 ubuntu ubuntu     0 Sep 12  2024 .Xresources

\-rw-r--r--  1 ubuntu ubuntu   111 Oct  3  2024 .apport-ignore.xml

\----------

\--------------------

drwxr-xr-x  2 ubuntu ubuntu  4096 Feb 27  2022 Templates

drwxr-xr-x  2 ubuntu ubuntu  4096 Feb 27  2022 Videos

drwxr-xr-x  4 ubuntu ubuntu  4096 Dec 11 12:29 logs

drwxr-xr-x  5 ubuntu ubuntu  4096 Dec 11 12:29 projects

drwx------  3 ubuntu ubuntu  4096 Sep 12  2024 snap

Hidden files aren't really secret; they start with a dot ., and Linux hides such files by default.



Step-3 (Let’s Move Around) :-

\---------------------------

To walk through the filesystem, we can use: cd <directory>. For example: cd Documents, and this will change our directory to Documents, as shown below





cd Command

ubuntu@tryhackme:\~$ cd Documents/

ubuntu@tryhackme:\~/Documents$ pwd

/home/ubuntu/Documents

To go "back" one level, we will use the command cd .., as shown below:





cd

Command

ubuntu@tryhackme:\~/Documents$ cd ..

ubuntu@tryhackme:\~$ pwd

/home/ubuntu



Step-4 (Learn the Power of "Find") :-

\----------------------------------

Let's now use one of the handy tools to find. As the name suggests, this built-in utility is used to locate files within the file system. Here's a simple version of the command: find <starting\_point> -name <filename>. Since your supervisor mentioned that the file mission\_brief.txt resides somewhere in your home directory, begin the home directory symbol: \~. So we will run the command: find \~ -name mission\_brief.txt, as shown below:





find Command

ubuntu@tryhackme:\~$ find \~ -name mission\_brief.txt

/<REDACTED-PATH>/mission\_brief.txt

Please note that this may take a moment, as Linux will check every folder inside your home directory. If the file exists, Linux will print the full path to it. The above result shows that the command has successfully located the file and provided us with its complete path, allowing us to navigate and read the file's content.



Let's use the cd command to navigate to the folder. We can also do ls to confirm the presence of the file, as shown below:





cd Command

ubuntu@tryhackme:\~$ cd /<REDACTED-PATH>/

ubuntu@tryhackme:\~/<REDACTED-PATH>$ ls

mission\_brief.txt



Step-5 (Read the File) :-

\----------------------

Another useful utility is cat. This is used to read the content of the file. To read this file, we will run the command cat mission\_brief.txt to get the content, as shown below:





cat Command

ubuntu@tryhackme:\~/<REDACTED-PATH>$ cat mission\_brief.txt

Great job finding your way around the terminal.



Your next assignment is to collect a small system report:

\- Who you're logged in as

\- The kernel version

\- Total disk space

\- The name of this Linux distribution



Once you gather those details, you'll be ready for the next step.



FLAG:<REDACTED>



Lab :-

\----

summarization of Lab solve steps :-

\--------------------------------

Step-1 (List directory contents to explore the home directory) :-

\---------------------------------------------------------------

Checking visible files in the current folder.ls is short for list. It displays the non-hidden files and directories located inside your current working directory (/home).

Bash

ls

ls: The base command to list directory contents.

Output: ubuntu (shows the user home directory named ubuntu).



Step-2 (Display detailed and hidden file information) :-

\------------------------------------------------------

Checking permissions and hidden files using flags.ls -la lists all contents including hidden files (files starting with a dot .) alongside detailed information like permissions, owner, group, size, and modification date.

Bash

ls -la

ls: The list command.

\-l: Long listing format (shows permissions, owner, file size, and timestamps).

\-a: All files (includes hidden files and directories starting with .).



Step-3 (Check directory properties without listing contents) :-

\-------------------------------------------------------------

Verifying the permissions of the current directory itself.

ls -ld displays details about the directory itself (.) rather than listing what is inside it.

Bash

ls -ld

\-l: Long listing format.

\-d: Directory option (tells ls to list the directory itself, not its contents).

.: Represents the current directory (/home).



Step-4 (Search for specific hidden target files) :-

\-------------------------------------------------

Using pattern matching to locate hidden clues. The find command searches for files in a directory hierarchy based on specified criteria like name, type, or size.Bashfind /home -name '.hidden\_clue'

find: The command used to search for files and directories.

/home: The starting directory path where the search begins.

\-name: Flag indicating search by exact filename.

'.hidden\_clue': The specific filename target enclosed in quotes to avoid shell expansion.Result: /home/ubuntu/.hidden\_clue



Step-5 (Locate the mission brief file using a relative search) :-

\---------------------------------------------------------------

Finding the exact path to answer Question 1. Search relative to the current directory (/home) to locate mission\_brief.txt.

Bash

find . -name 'mission\_brief.txt'

.: Represents the current working directory (/home).

\-name 'mission\_brief.txt': Tells find to search specifically for a file named mission\_brief.txt.

Result: ./ubuntu/Documents/.research/archive/mission\_brief.txt

Full Path (Answer to Question 1): /home/ubuntu/Documents/.research/archive/mission\_brief.txt



Step-6 (Read the target file contents to retrieve the flag) :-

\------------------------------------------------------------

Reading file text to answer Question 2.cat (short for concatenate) reads data from the specified file and prints its contents directly to the terminal output.

Bash

cat ./ubuntu/Documents/.research/archive/mission\_brief.txt

cat: The command used to output file contents to the terminal.

./ubuntu/Documents/.research/archive/mission\_brief.txt: The target file path to print.

Flag Found (Answer to Question 2): MISSION-FOUND



Answer the questions below:

What is the full path of the mission\_brief.txt file found on the system using the find command?



Answer : /home/ubuntu/Documents/.research/archive/mission\_brief.txt



What is the flag hidden inside the mission\_brief.txt file?



Answer : MISSION-FOUND



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Investigating the System :-

\-------------------------

your supervisor wants you to gather some basic information about the system you’re working on. This kind of information helps cyber security teams understand what environment they’re operating in, what version of Linux they’re using, and what resources are available.



Think of this as taking a quick health check of the machine.



Your Next Assignment

When you opened mission\_brief.txt, it contained a new message:



Great job finding your way around the terminal. Your next assignment is to collect a small system report:



Who you're logged in as

The kernel version

Total disk space

The name of this Linux distribution

You’re still on your own for now, but at least the instructions are clear: collect system info and send it back. Let’s break the job into small steps.



Step-1 (Who Are You Logged in As?) :-

\-----------------------------------

The simplest command in Linux also happens to be one of the most useful: whoami





whoami Command

ubuntu@tryhackme:\~$ whoami

ubuntu

This prints your current username.



Step-2 (What System Are You On?) :-

\--------------------------------

To see details about the operating system, kernel version, and architecture, use: uname -a





uname -a Command

ubuntu@tryhackme:\~$ uname -a

Linux tryhackme <REDACTED>-aws #17-Ubuntu SMP Mon Sep  2 13:48:07 UTC 2024 x86\_64 x86\_64 x86\_64 GNU/Linux

This gives a full line of system information - great for understanding exactly what environment you're working in.



Breakdown of the Information



* Linux: The system is running the Linux kernel.
* tryhackme: The hostname (the computer’s name).
* <REDACTED>-aws: The kernel version installed on the machine.
* x86\_64: The hardware platform (also 64-bit).
* GNU/Linux: The operating system type (Linux kernel + GNU tools).

If you only want the operating system name, you can try: uname





uname Command

ubuntu@tryhackme:\~$ uname

Linux

But for now, uname -a gives the fuller picture.



Step-3 (Check Disk and Storage Info) :-

\-------------------------------------

In real-world environments, you’ll often need to check disk usage or available space, especially before running tools or analyzing logs. A simple command for readable output is: df -h





df -h Command

ubuntu@tryhackme:\~$ df -h

Filesystem      Size  Used Avail Use% Mounted on

/dev/root        --G   12G   --G  17% /

tmpfs           1.9G     0  1.9G   0% /dev/shm

tmpfs           774M  1.2M  773M   1% /run

tmpfs           5.0M     0  5.0M   0% /run/lock

tmpfs           387M  192K  387M   1% /run/user/1000

tmpfs           387M  172K  387M   1% /run/user/114

The -h means "human readable"; it shows sizes like 2G or 500M instead of long bytes-only numbers.



Breakdown of the Information



* /dev/root is the main disk of the system with --G total, 12G used, <REDACTED>G free, and is 17% full.
* tmpfs entries are temporary filesystems stored in RAM, not on the physical disk.
* /dev/shm is a shared memory area with 1.9G available and 0 used.
* /run/user/114 is similar temporary storage for another system user, also 387M total and mostly empty.



Step-4 (Read a System File) :-

\----------------------------

Linux stores configuration and informational files in the /etc directory.

To practice navigating and reading files, head into /etc by running cd /etc and then list what’s inside: ls





cd Command

ubuntu@tryhackme:\~$ cd /etc

ubuntu@tryhackme:/etc$ ls

ImageMagick-6                  cloud                 firefox               hp               logcheck              opt                     rmt                sysctl.d

ModemManager                   compizconfig          fonts                 ifplugd          login.defs            os-release              rpc                sysstat

NetworkManager                 console-setup         fstab                 init             logrotate.conf        overlayroot.conf        rsyslog.conf       systemd

\---

\-------

chatscripts                    ethertypes            hosts.deny            localtime        openvpn               resolv.conf             sysctl.conf

ubuntu@tryhackme:/etc$

Let’s now use cat to read the os-release file that almost every Linux system contains: cat os-release, as shown below:





&#x20;cat Command

ubuntu@tryhackme:/etc$ cat os-release

PRETTY\_NAME="Ubuntu 24.04.1 LTS"

NAME="Ubuntu"

VERSION\_ID="24.04"

VERSION="24.04.1 LTS (Noble Numbat)"

VERSION\_CODENAME=noble

ID=ubuntu

ID\_LIKE=debian

HOME\_URL="https://www.ubuntu.com/"

SUPPORT\_URL="https://help.ubuntu.com/"

BUG\_REPORT\_URL="https://bugs.launchpad.net/ubuntu/"

PRIVACY\_POLICY\_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"

UBUNTU\_CODENAME=noble

LOGO=ubuntu-logo

This file provides details about the Linux distribution that are often clearer than those provided by the uname command.



Great work. With just a few commands, we were able to retrieve the system information as requested by the supervisor.



Wrapping Up Your First Day :-

\--------------------------

You’ve navigated the filesystem, searched for hidden files, and gathered system information, solid progress for your first steps into Linux. Before you finish your day, your supervisor has left one final task to test everything you’ve learned so far.

Nothing too hard, just a quick check to make sure you can put the basics together on your own.



Mini Challenge :-

\--------------

You only know the name of the file: day1\_report.txt



Your job :-

\---------

1. Use the find command to locate it somewhere in your home directory.

2\. Navigate to the folder where it was found.

3\. Read the file contents using cat.

4\. Use it for the the last question in this task.



Lab :-

\----

Step-1 (Check your current username) :-

\-------------------------------------

Identifying the current logged-in user.

The whoami command prints the effective username of the person currently logged into the terminal session.

Bash

whoami



* whoami: The base command to display the current user.
* Username Found (Answer to Question 1): ubuntu



Step-2 (Display full system information) :-

\-----------------------------------------

Retrieving system and kernel details.

The uname command displays detailed system information.

Adding the -a flag prints everything it knows, including the kernel version.

Bash

uname -a



* uname: The command to get system information (Unix Name).
* \-a: Stands for "all", telling the system to display the kernel name, network hostname, kernel release, and OS details.
* Kernel Version Found (Answer to Question 2): 6.14.0-1018-aws



Step-3 (Report file system disk space usage) :-

\---------------------------------------------

Checking available disk capacity.

The df command reports file system disk space usage.

Using the -h flag makes the output human-readable (Megabytes and Gigabytes instead of raw blocks).



Bash

df -h



* df: Short for "disk free", it shows total and available disk space.



* \-h: "Human-readable" option to display sizes in G (Gigabytes) or M (Megabytes).



* Free Disk Space Found (Answer to Question 3): 58G (Available on the /dev/root filesystem).



Step-4 (Locate the target file in your home directory) :-

\------------------------------------------------------

Searching for the report file. After attempting to open the file directly and failing, the find command is used to search the entire home directory to locate exactly where the report is hidden.



Bash

find \~ -name 'day1\_report.txt'



* find: The command used to search for files and directories.



* \~: A shortcut symbol representing your home directory (/home/ubuntu).



* \-name 'day1\_report.txt': Tells the system to search exactly for this filename.



* Result: /home/ubuntu/.logs/archive/day1\_report.txt



Step-5 (Read the report contents to retrieve the message and flag) :-

\------------------------------------------------------------------

Reading file text to answer Question 4.Once the exact path is found, cat reads the file and prints its text directly to your screen.



Bash

cat /home/ubuntu/.logs/archive/day1\_report.txt



* cat: Short for concatenate, used here to output the file's contents.



* /home/ubuntu/.logs/archive/day1\_report.txt: The full hidden path to the file.



* Message/Flag Found (Answer to Question 4):

Well done! You've completed all tasks for today.

You're starting to get comfortable with the terminal – keep practicing.

Your next set of challenges will build on what you learned here.

FLAG:END-OF-DAY1



Answer the questions below:

What is the username returned by the whoami command?



Answer : ubuntu



What is the kernel version shown by uname -a?



Answer : 6.14.0-1018-aws



How much free disk space does df -h report?



Answer : 58G



What is the message written inside day1\_report.txt?



Answer : END-OF-DAY1



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conclusion :-

\-----------

And that’s your first day on the Cyber Operations Support Team.



You learned how to :-

\-------------------



* Navigate the Linux filesystem
* Search for files
* Inspect system information
* Read important configuration files
* Follow clues and complete missions inside a Linux environment

These skills may seem simple, but they’re the building blocks for everything that comes later: file permissions, users \& groups, processes, package management, and eventually real security tooling.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Windows CLI Basics :-

\------------------

Task 1 :-

\-------

Introduction :-

\-------------

In the previous Linux CLI Basics room, you took your first steps into the Linux command line. Today, you're continuing your journey, but this time on Windows. Windows is one of the most widely used operating systems in workplaces worldwide. As someone interested in cyber security, you will often investigate or troubleshoot Windows machines, especially user desktops and laptops.



In this room, you'll learn how to use the Windows Command Prompt to navigate files, search for information, and gather basic system details using the same hands-on, story-driven approach as before.



From a security perspective, Windows is important because many real-world attacks and investigations involve Windows systems.



What Is the Windows Command Line?



Answer : The Command Prompt (often referred to as CMD) is a text-based interface for interacting with the Windows operating system. Instead of clicking folders and menus, you type commands to tell the system exactly what you want to do, such as listing files, moving between folders, or checking system information. It might look simple, but it's a powerful and widely used tool.



Learning Objectives :-

\--------------------

By the end of this room, you will be able to:



* Use the Windows command line confidently
* Navigate folders without clicking
* Find files when you only know their name
* Read files using the terminal
* Collect basic system and network information

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Windows CLI :-

\-----------

Step-1 (Where Am I?) :-

\--------------------

Before doing anything else, open the terminal on the Desktop, and check your current location by typing the command cd, as shown below:



Shows output of cd command



This shows the full path of the directory you're currently in. On Windows, this is usually your user folder. Please note that the cd command is also used to change the directory, which we will use later in the task.



Step 2 (What's Around Me?) :-

\--------------------------

Now, list the contents of the current directory using the command: dir



This command will list down the files and the folders present in the current directory, as shown below:



Shows output of dir command



You'll see files and folders that are visible by default. Take a moment to look around; not everything you need will always be obvious. From the output, we can see that the command has returned 16 directories.



Step 3 (Are There Hidden Files?) :-

\--------------------------------

Some files and folders on Windows are marked as hidden, which means they don't appear in a normal listing. To show everything, including hidden items, run: dir /a



Shows output of dir/a command



The output clearly indicates that more than 12 hidden folders were found. It is important to note that hidden doesn't mean secret; it just means Windows hides them by default.



Step 4 (Moving Around the Filesystem) :-

\-------------------------------------

Let's use the cd command to navigate through the folders. We can use the format cd folder\_name to move to the specified folder. The command cd Documents will move us to the Documents folder, as shown below. To move back one level, we can use the cd command.



Shows the output of cd command



To become familiar with the environment, use the dir or dir /a command to move to see what's inside each folder. You can explore a few folders to get comfortable, but the file you're looking for probably isn't in an obvious place.



Step 5 (Finding the File on the Disk) :-

\-------------------------------------

Instead of guessing where the file is, let Windows search for it. Use the following command: dir /s task\_brief.txt. The /s flag tells Windows to search all subfolders starting from your current directory and show you the full path if the file exists.



Shows the command to search for the files on the system



As we can see, the command above helped us locate the file and provided its full path. Take note of the path shown in the output.



Step 6 (Navigate to the File) :-

\-----------------------------

Now that we know where the file is located, let's use the cd command to navigate to the folder using the command format cd <path\_to\_the task\_brief.txt>. Use dir again to confirm that task\_brief.txt is in the folder, as shown below:



Shows output of the cd command



Step 7 (Read the File) :-

\----------------------

Now read the contents of the file using: type task\_brief.txt. This will print the contents of the file directly in the command prompt, as shown below:



Shows the use of type command to read the file content



Perfect.



You have not only learned how to navigate Windows directories using the CLI, but also how to find files and read their contents.



The content of task\_brief.txt leads us to our next task: inquiring about the system we are currently using. Let's explore that in the next task.



Lab :-

\----

Step-1 :-

\------

we first open cmd as a administrator

step-2 :-

\------

now we give the dir command to see in current location what folders are present and use dir /a for see in each folder what inside they have.

Step-3 :-

\-------

here we go first the Documents folder so to go documents folder we give command cd documents

Step-4 :-

\-------

next we need to go find task\_brief.txt but we don't know in c drive in documents folder in which subfolder inside that is present so we run command dir /s task\_brief.txt so it serach automatically in documents folder inside all subfolder where that file is located.

Step-5 :-

\------

Now we found that under documents in which location that txt file is present C:\\Users\\Administrator\\Documents\\Notes\\research\_yn6\\exports\_imv\\screenshots\\notes\_wi6.so now we use that location to reach our file so to do that we run command cd C:\\Users\\Administrator\\Documents\\Notes\\research\_yn6\\exports\_imv\\screenshots\\notes\_wi6

Step-6 :-

\-------

Now we give dir command in the following location to get final confirmation that our txt file there so we run command dir again.

Step-7 :-

\------

now to read the txt file we run command type task\_brief.txt and after the command give we see that txt file inside content and get our flag and give the 2nd questions answer.



Answer the questions below:

1. What is the full path of the task\_brief.txt found on the system?



Answer : C:\\Users\\Administrator\\Documents\\Notes\\research\_yn6\\exports\_imv\\screenshots\\notes\_wi6

\-------



2\. What message and flag are written inside task\_brief.txt?



Answer : TASK-BRIEF-FOUND

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

Gathering System Information on Windows :-

\---------------------------------------

Overview :-

\--------

Now that you know how to move around and find files using the Windows command line, it’s time to learn how to ask the system questions about itself. cyber security and IT professionals do this all the time. Before fixing a problem or investigating an incident, they first want to know:



* Who am I logged in as?
* What machine is this?
* What version of Windows is it running?
* How is it connected to the network?

In this task, you'll learn how to gather that information step by step.



Step-1 (Who Am I Logged In As?) :-

\-------------------------------

When working on a system, one of the first things to check is which user account you’re using. This matters because different users can have different permissions.



Run the following command:

whoami (This command prints the username of the account you’re currently logged into.)



Shows output of whoami



Step-2 (What Is the Name of This Computer?) :-

\--------------------------------------------

Every Windows machine has a name. In workplaces, this helps identify network systems. To see the computer’s name, run: hostname.







You’ll see a short name printed in the terminal.



Step-3 (What Version of Windows Is This?) :-

\------------------------------------------

Next, let’s look at details about the operating system itself. Run:systeminfo



This command prints a lot of information. Don’t worry, you’re not expected to understand everything yet.



Focus on these parts:



* OS Name
* OS Version
* System Type

These details indicate the version of Windows the machine is running and whether it’s 32-bit or 64-bit.



Step-4 (How Is This Machine Connected to the Network?) :-

\------------------------------------------------------

Finally, let’s look at basic network information. Run: ipconfig



This shows the machine's network configuration.



Look for :-

\--------



1. An IPv4 Address

2\. A Default Gateway



This information helps analysts understand how a machine connects to the network.



Summary :-

\-------

In this task, you learned how to ask a Windows system simple but important questions using the command line.



You practiced :-

\-------------



* Identifying who you are logged in as
* Finding the name of the computer
* Checking Windows version and system details
* Viewing basic network information

These are some of the first commands analysts and IT staff run when they start working on a Windows machine.



Lab :-

\----

Step-1 :-

\-------

First we open cmd as a administarator

Step-2 :-

\-------

Now we give command hostname so computer name come that is thmlab in output give so we place it as a answer of first question and our first question is solve.

Step-3 :-

\-------

now we run systeminfo command in cmd that give various information like example OS name, OS version, OS Manufacturer, OS Build type, Registered owner, Registered organization, Product ID, Original install date, system Boot Time, System manufacturer, System model, System type , processor, BIOS version, windows directory, System Directory, Boot device, System locale, Boot locale, Time zone, Physical memory, available physical memory, Virtual memory max size and Virtual memory available, Virtual memory in use, page file location, Domain ,logon server, Hotfix(s), Network cards, Hyper-v requirements so in them we just need to solve the 2nd question see OS version detail and that is here 10.0.17763 N/A Build 17763. So we place it as a answer of 2nd question and our 2nd question is that's how solved.



Answer the questions below:

What is the computer name shown by hostname?



Answer : thmlab



What Windows version is listed in the systeminfo output?



Answer : 10.0.17763 N/A Build 17763

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conclusion :-

\----------

Overview :-

\---------



In this room, we learned how to interact with a Windows system using the command line instead of relying on the graphical interface. This task is a short wrap-up to reflect on what you’ve learned and why it’s important.



What You Learned :-

\-----------------

In this room, you practiced using the Windows Command Prompt to:



* Navigate files and folders without clicking
* Locate files even when you didn’t know where they were
* Reveal hidden files and directories
* Read file contents directly from the terminal
* Gather basic system and network information
* 

These are foundational skills that apply across many roles in IT and cybersecurity.



Why This Matters ?

In real-world environments :-

\--------------------------



* Not everything is visible in the graphical interface
* Files may be hidden or buried deep in the system
* Analysts often need quick answers without clicking through menus
* Command-line tools are faster, more precise, and easier to automate
* Being comfortable with the Windows command line gives you more control and better visibility into a system.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Operating System Security Room :-

\------------------------------

Task 1 :-

\-------

Introduction to Operating System Security :-

\-----------------------------------------

Every day you use a smartphone or a laptop or almost any type of computer, you interact directly or indirectly with an operating system. Operating systems include MS Windows, macOS, iOS, Android, Chrome OS, and Linux. But what is an operating system? To define an operating system, we need to visit one computer term: hardware.





Computer hardware refers to all the computer parts and peripherals that you can touch with your hand. Hardware includes the screen, the keyboard, the printer, the USB flash memory, and the desktop board. As shown in the figure below, the desktop board contains many components, in particular, a central processing unit (CPU) and memory chips (RAM). Although not shown in the image below, the desktop board is usually connected to a storage device (HDD or SSD).





The desktop board is the main part of a computer, and all the other pieces of hardware from keyboard and mouse to screen and printer connect to it. However, hardware components by themselves are useless if you want to run your favorite programs and applications. We need an Operating System to control and “drive” them.



Software and hardware :-

\---------------------



The Operating System (OS) is the layer sitting between the hardware and the applications and programs you are running. Example programs you would use daily might include a web browser, such as Firefox, Safari, and Chrome, and a messaging app, such as Signal, WhatsApp, and Telegram. All the programs and applications cannot run directly on the computer hardware; however, they run on top of the operating system. The operating system allows these programs to access the hardware according to specific rules.



Some operating systems are designed to run on laptops and personal desktops, such as MS Windows 11 and macOS. Other operating systems are designed specifically for smartphones, such as Android and iOS. There are also operating systems intended for servers; examples include MS Windows Server 2022(opens in new tab), IBM AIX(opens in new tab), and Oracle Solaris(opens in new tab). Finally, there are operating systems that you can use on a personal computer and server; one example is Linux. The image below shows the popularity of the different operating systems used to browse the Internet according to Statcounter(opens in new tab) based on the data collected during January 2022.







Your smartphone might be running Android or iOS, and you might have plenty of private data on it. Examples include:



* Private conversations with your family and friends
* Private photos with family and friends
* Email client that you use for personal and work communications
* Passwords saved in the web browser (or even in notes)
* E-banking apps
* The list of confidential and private data goes on. You don’t want someone you don’t trust to open your phone and go through your photos, conversations, and apps. Hence, you need to secure your phone and its operating system.



The same goes for your laptop or computer running MS Windows, macOS, or Linux. Your computer will most likely contain plenty of information such as:



* Confidential files related to your work or university
* Private personal files, such as a copy of your ID or passport
* Email programs, such as MS Outlook and Mozilla Thunderbird
* Passwords saved in web browsers and other apps
* Copy of digital camera and smartphone photos



The list can get very long, depending on the type of user. And considering the nature of the saved data, you want to ensure that your data is secure. When we talk about security, we should think of protecting three things:



1. Confidentiality :-

&#x20;  ----------------

You want to ensure that secret and private files and information are only available to intended persons.

2\. Integrity :-

&#x20;  ---------

It is crucial that no one can tamper with the files stored on your system or while being transferred on the network.

3\. Availability :-

&#x20;  -------------

&#x20;You want your laptop or smartphone to be available to use anytime you decide to use it.

&#x20;

Answer the questions below:

Which of the following is not an operating system?



AIX

Android

Chrome OS

Solaris

Thunderbird

Answer : Thunderbird

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Common Examples of OS Security :-

\-------------------------------

As we mentioned in the previous task, security is concerned with attacks against:



* Confidentiality
* Integrity
* Availability

In this room, we will focus on three weaknesses targeted by malicious users :-



* Authentication and Weak Passwords
* Weak File Permissions
* Malicious Programs
* Authentication and Weak Passwords

Authentication is the act of verifying your identity, be it a local or a remote system. Authentication can be achieved via three main ways:



1. Something you know, such as a password or a PIN code.

2\. Something you are, such as a fingerprint.

3\. Something you have, such as a phone number via which you can receive an SMS message.



Since passwords are the most common form of authentication, they are also the most attacked. Many users tend to use easy-to-guess passwords or the same password on many websites. Moreover, some users rely on personal details such as date of birth and name of their pet, thinking that this is easy to remember and unknown to attackers. However, attackers are aware of this tendency among users.



The National Cyber Security Centre (NCSC) has published a list of the 100,000 most common passwords(opens in new tab). Let’s look at the top 20 passwords in the table below.



|Rank|Password|
|-|-|
|1|123456|
|2|123456789|
|3|qwerty|
|4|password|
|5|111111|
|6|12345678|
|7|abc123|
|8|1234567|
|9|password1|
|10|12345|
|11|1234567890|
|12|123123|
|13|000000|
|14|iloveyou|
|15|1234|
|16|1q2w3e4r5t|
|17|qwertyuiop|
|18|123|
|19|monkey|
|20|dragon|



We can see that 123, 1234, 12345, …, 123456789, and 1234567890 are on the list. Dictionary words such as password, iloveyou, monkey, and dragon are commonly used. Words not in the dictionary include qwerty, qwertyuiop, and 1q2w3e4r5t; these seemingly complex passwords are very predictable as they follow the keyboard layout.



In brief, if the attacker can guess the password of any of your online accounts, such as your email or social media account, they will be able to gain access to your private data. Therefore, it is vital that you choose complex passwords and use different passwords with different accounts.



Weak File Permissions :-

\----------------------

Proper security dictates the principle of least privilege. In a work environment, you want any file accessible only by those who need to access it to get work done. On a personal level, if you are planning a trip with family or friends, you might want to share all the files related to the trip plan with those going on that trip; you don’t want to share such files publicly. That’s the principle of least privilege, or in simpler terms, “who can access what?”



Weak file permissions make it easy for the adversary to attack confidentiality and integrity. They can attack confidentiality as weak permissions allow them to access files they should not be able to access. Moreover, they can attack integrity as they might modify files that they should not be able to edit.



Access to Malicious Programs :-

\-----------------------------

The last example we will consider is the case of malicious programs. Depending on the type of malicious program, it can attack confidentiality, integrity, and availability.



Some types of malicious programs, such as Trojan horses, give the attacker access to your system. Consequently, the attacker would be able to read your files or even modify them.



Some types of malicious programs attack availability. One such example is ransomware. Ransomware is a malicious program that encrypts the user's files. Encryption makes the file(s) unreadable without knowing the encryption password; in other words, the files become gibberish without decryption (reversing the encryption). The attacker offers the user the ability to restore availability, i.e., regain access to their original files: they would give them the encryption password if the user is willing to pay the “ransom.”



Answer the questions below:

Which of the following is a strong password, in your opinion?



iloveyou

1q2w3e4r5t

LearnM00r

qwertyuiop

Answer : LearnM00r

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Practical Example of OS Security :-

\--------------------------------

In one typical attack, the attacker seeks to gain access to a remote system. We can accomplish this attack by tricking the target into running a malicious file or by obtaining a username and a password. We will focus on the latter. After discovering a username, we will try to “guess” the password; furthermore, we will try to escalate our privileges to a system administrator. This account is called root on Android, Apple, and Linux systems. While, on MS Windows systems, this account is called administrator. The accounts root and administrator have complete unrestricted access to a system.







In this task, we will try to hack into a Linux system. We assume that you have never used a Linux system before, and we will explain accordingly.



Start the AttackBox by clicking on the “Start AttackBox” button at the top left of the room. Start the attached machine by clicking on the green “Start Lab Machine” button at the top right of this task. It usually takes a minute or two to load fully. Once they are both ready, you should use the AttackBox, which should be taking the right half of your screen by now.



On the AttackBox, start the terminal by clicking on the terminal icon shown in the image above. You will be writing all the commands you need on the terminal shown below.



Step-1 (Establish Initial Access via SSH) :-

\-----------------------------------------

Authenticate using the leaked credentials. Use Secure Shell (SSH) to connect to the target machine using the credentials found during physical reconnaissance.



Bash

ssh sammie@10.48.190.243



* Certificate Warning :-

&#x20;  -------------------

If this is your first time connecting to this host, the system will prompt you to verify the server's authenticity. Type yes to accept the ECDSA key fingerprint. Password Entry: Enter the password dragon. The terminal will not display asterisks or characters for security reasons, but it is registering your keystrokes. Press Enter to submit.



* Password Entry :-

&#x20;  ---------------

Enter the password dragon. The terminal will not display asterisks or characters for security reasons, but it is registering your keystrokes. Press Enter to submit.



Step-2 (Verify User Context) :-

\----------------------------

Confirm session privileges. Once connected, verify your current session privileges to ensure you are operating as the intended user.

Bash

whoami

This should return sammie.



Step-3 (Enumerate the Directory) :-

\--------------------------------

List visible files and folders. Perform basic reconnaissance of your current working directory to identify potential targets of interest.

Bash

ls

This reveals available files such as country.txt, draft.md, icon.png, password.txt, and profile.jpg.



Step-4 (Inspect File Contents) :-

\------------------------------

Read plaintext data. Use the concatenate command to output the contents of specific text files directly to your terminal screen.

Bash

cat draft.md

Pro-tip: Always check files named password.txt or similar variants immediately during an assessment.



Step-5 (Review Command History) :-

\--------------------------------

Check for operational security failures. Analyze the current user's command history. This is a critical post-exploitation step to uncover hardcoded passwords, hidden directories, or previous administrative actions.

Bash

history



Step-6 (Execute Lateral Movement) :-

\---------------------------------

Attempt to compromise additional accounts. The environment contains two other users known for poor security practices: johnny and linda. You can attempt a manual password guessing attack using one of two methods:



* Method A (From your current SSH session) :-

&#x20;  ----------------------------------------

Use the substitute user command to switch directly without dropping your connection.

Bash

su - johnny



* Method B (From your local AttackBox) :-

&#x20;  -------------------------------------

Open a new terminal tab and initiate a fresh SSH connection attempt.

Bash

ssh johnny@10.48.190.243



Lab :-

\----

Step-1 :-

\------

First we give command from our attack box to victim machine ip (10.48.190.243) to connect through ssh and also the the user that present already in victim machine so here we need ip and username of victim machine by connect through ssh protocol. So we give command  ssh sammie@10.48.190.243.



Step-2 :-

\------

now we see sammie@10.48.190.243 and give command whoami and we see the username Sammie.



Step-3 :-

\------

now give ls -al command to see the existed files and directories even if hidden so here we get to important file named password.txt and country.txt.



Step-4 :-

\------

Now give command cat password.txt where get two this user Sammie password dragon and Sammie and another when give cat country.txt we found uk.



Step-5 :-

\------

Now we try to login in jhonny user in victim machine to Sammie user so we give command su - johnny and password we try national cyber security center published 20 common password one by one and we found that one of them abc123 password is used to login for jhonny user so we successfully able to login as jhonny user. So here we give first questions answer that jhonny user password is abc123.



Step-6 :-

\------

Now jhonny user type mistakenly root user password in terminal and we anyhow know it or guess it or just normally out of curiosity we give command history to find a way to get root user password and login as root. there we found a password named happyHack!NG so we next time try it. So that's how we give second question answer that what is root user password so root user password is happyHack!NG.



Step-7 :-

\------

Now we try to login as root so we give command su -root and password give happyHack!NG and we able to successfully login as root. Now we go to root directory so we first give command cd.. and we back in root home then again give cd .., now we back to main root / this location root@ip-10-48-107-249:/#.



Step-8 :-

\-------

Now we give ls command and we see root directory we now try to go first root directory so to do that we give command  root@ip-10-48-107-249:/# cd root and we redirect to the root directory and now our location is -----

&#x20;root@ip-10-48-107-249:\~# pwd

/root



Step-9 :-

\-------

Now here we want to see what files and directories present in that /root directory so we give command again ls -al and finally we found flag.txt, Now we just to see it inside content give command cat flag.txt and we found the flag THM{YouGotRoot} and that is our final third questions answer that we found so finally our the final questions answer we found and lab is solve.

Answer the questions below:

Based on the top 7 passwords, let’s try to find Johnny’s password. What is the password for the user johnny?



Answer : abc123



Once you are logged in as Johnny, use the command history to check the commands that Johnny has typed. We expect Johnny to have mistakenly typed the root password instead of a command. What is the root password?



Answer : happyHack!NG



While logged in as Johnny, use the command su - root to switch to the root account. Display the contents of the file flag.txt in the root directory. What is the content of the file?



Answer : THM{YouGotRoot}

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data Representation Room :-

\-------------------------

Task 1 :-

\-------

Introduction :-

\------------

Are you curious to explore in-depth how computers represent colors and numbers? You are not only interested in seeing a purple color on the screen, but also interested in inspecting how this “purple” is represented in the computer memory. As a bonus, you will also learn how computers manage to do all their calculations when they can read and write only two states and interpret them as 0 and 1.



One lamp is on with 1 written on it. The other is off with 0 written on it.



Human beings find it most convenient to use the decimal system for everyday tasks, such as counting, measuring, weighing, and paying. If you like jogging, you might track your progress by timing yourself; for instance, you might say you jogged for 23 minutes. When you look at prices, you expect something like 17, 99, 239, 3049, and so on. Without giving it much thought, we use the decimal system, where the digits range from 0 to 9. Computers, on the other hand, are limited to two digits: 0 and 1. If you have ever wondered how computers represent the different values using only two digits, this room will help you get some answers.



Learning Objectives :-

\--------------------

* Representing 8 colors
* Representing 16 million colors
* Binary numbers
* Hexadecimal numbers
* (Optional) Octal numbers



After you finish this room, you will have a solid understanding of how computers represent colors and understand numbers (specifically positive integers). Being familiar with binary and hexadecimal system representations is a must when you use various computer tools, especially in the domain of cyber security.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Representing Colors :-

\-------------------

Our First Eight Colors By combining different amounts of red, green, and blue lights, you can get any color you like. In computer colors, think of it like three knobs, and each knob controls one of the three colors.



Example :-

\--------



Let’s say that each of the three colors can be either on or off, i.e., each has two states.



1. The red light can be either on or off

2\. The green light can be either on or off

3\. The blue light can be either on or off

4\. These states give us 2 × 2 × 2 = 8, that’s eight different colors.

5\. 3 circles (red, green, and blue) overlapping.



If a computer were limited to 8 colors, it would only need to indicate which color is “switched on” and which is “switched off.” In fact, it can use three digits of 1 and 0 to represent the states of red, green, and blue. For example, 111 would be all 3 lights switched on, while 100 would be only the red switched on. This digit, which can be either 1 or 0, is called a bit.



Now, a computer can represent any of the 8 colors. If this is still unclear, a detailed list is shown in the table below.



|Color Representation|Representation Meaning|Color Name|
|-|-|-|
|000|All colors are off|Black|
|001|Only blue is on|Blue|
|010|Only green is on|Green|
|100|Only red is on|Red|
|011|Green and blue are on|Cyan|
|101|Red and blue are on|Magenta|
|110|Red and green are on|Yellow|
|111|All colors are on|White|



We just provided a way to represent a color in a palette of 8 colors.



From 8 to 16,000,000 :-

\---------------------

Being limited to eight colors is inconvenient, as we prefer millions of colors. It would be convenient if each of the 3 lights (red, green, and blue) had 256 levels instead of just 2 (on or off). Let’s repeat the same math as earlier: 256 × 256 × 256 = 16,777,216. That’s more than 16 million colors; that covers most of our needs.



One bit is enough to represent 2 states: on and off. We need 8 bits to express 256 states. In most textbooks, a group of 8 bits is referred to as a byte; however, you can also use the term octet.



Putting all this together, you would realise that a color is now represented as 3 × 8 bits, or 3 bytes (24 bits). For example, one green color used on this page is represented as 10100011 11101010 00101010; that’s not a very convenient way to type or read color codes. Here comes the hexadecimal representation to the rescue!



Hexadecimal Representation :-

\---------------------------

Hexadecimal representation makes it easy to combine 4 bits into a single character, a hexadecimal digit, to be specific. For now, please think of the hexadecimal digits as symbols where each symbol represents a set of 4 bits. We will revisit hexadecimal numbers in Task 3.



|Hexadecimal Digit|Binary Representation|
|-|-|
|0|0000|
|1|0001|
|2|0010|
|3|0011|
|4|0100|
|5|0101|
|6|0110|
|7|0111|
|8|1000|
|9|1001|
|A|1010|
|B|1011|
|C|1100|
|D|1101|
|E|1110|
|F|1111|



Going back to the green color, instead of typing 10100011 11101010 00101010, we can type A3EA2A. In fact, that’s how you specify the color in graphics programs. For your convenience, the attached static site helps you convert a hex color into its binary and decimal representations, along with a color preview.



To summarise what we have covered so far :-

\-----------------------------------------



* In real-life applications, a color is represented in 24 bits, i.e., 3 bytes
* Each byte can represent 256 different values
* Each of the three bytes specifies the intensity of the red, green, and blue lights
* Every 4 bits are represented by one hexadecimal digit
* Each byte is represented as two hexadecimal digits



Lab :-

\----

Question 1 :-

\-----------

Enter Hex Color:

\#3BC81E

\-------

* Hexadecimal Representation:

&#x20;  3B C8 1E

* Binary Representation:

&#x20;  00111011 11001000 00011110

* Decimal Representation:

&#x20;  059 200 030



Question 2 :-

\-----------

Enter Hex Color:

\#EB0037

\-------

* Hexadecimal Representation:

&#x20;  EB 00 37

* Binary Representation:

&#x20;  11101011 00000000 00110111

* Decimal Representation:

&#x20;  235 000 055



Question 2 :-

\-----------

Enter Hex Color:

\#D4D8DF

\-------

* Hexadecimal Representation:

&#x20;  D4 D8 DF

* Binary Representation:

&#x20;  11010100 11011000 11011111

* Decimal Representation:

&#x20;  212 216 223



Answer the questions below:

1. Preview the color #3BC81E. In one word, what does this color appear to be?



Answer : green

\-------



2\. What is the binary representation of the color #EB0037?



Answer : 11101011 00000000 00110111

\-------



3\. What is the decimal representation of the color #D4D8DF?



Answer : 212 216 223

\-------

&#x20;

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Numbers: From Decimal to Hexadecimal :-

\-------------------------------------

Human beings have ten fingers, and this is the most plausible explanation for why we use the decimal (base-10) system in our everyday lives. Computers, on the other hand, have two fingers states that they understand:



* Low and High in voltage range (example: transistor-transistor logic)
* North and South in magnetic polarity (example: hard disk drives)
* Light presence (example: fiber optics)



Let’s consider the first example :-

\---------------------------------

On the electronic level, a transistor either passes or blocks electric current. Consequently, in all digital systems, everything boils down to a low or high state, representing 0 and 1, respectively. (For example, the low range can be voltage between 0 and 0.8 volts, while the high range is between 2 and 3.3 volts, or 2.7 and 5 volts, depending on the electronic system.) We are not affected by how the 0 and the 1 are represented on the physical level; however, we are concerned with how to use these two digits to represent data, such as numbers.



In the previous task, we saw that we can use a set of bits to fine-tune the steps. For instance, 1 bit can represent 2 states, while 8 bits can represent 256 states. In this task, we will learn a bit more about the math behind it; however, don’t worry if it appears complex at first glance. Things will make more sense as you progress in your learning journey.



In simple math terms, a number such as 213 is actually the same as saying 200 + 10 + 3. Isn’t this right?



In a more technical representation, 213 can be written as 213 = 2 × 102 + 1 × 101 + 3 × 100. As you would remember from the math class, 102 = 100, 101 = 10, and 100 = 1.



Consequently, this was just the formal mathematical way of saying 213 = 2 × 100 + 1 × 10 + 3 × 1. If you have not worked with math for some time, please give this some thought and a second read before you move on.



Binary Numbers :-

\--------------

The binary (base-2) system can be expressed similarly to what we wrote earlier, discussing the decimal (base-10) system. The key differences are that the binary system is limited to two digits, 0 and 1, and that everything is a power of 2. Let’s consider a couple of examples.



The binary number 1001 can be expressed as follows: 1001 = 1 × 23 + 0 × 22 + 0 × 21 + 1 × 20 = 1 × 8 + 0 × 4 + 0 × 2 + 1 × 1 = 8 + 0 + 0 + 1 = 9. We just demonstrated how to write 9 in binary.



Following the same approach, it won’t be challenging to convert the binary numbers 0000, 0001, 0010, 0011 to the decimal system. Let’s go through these four conversions.



0000 = 0 × 23 + 0 × 22 + 0 × 21 + 0 × 20 = 0 × 8 + 0 × 4 + 0 × 2 + 0 × 1 = 0



0001 = 0 × 23 + 0 × 22 + 0 × 21 + 1 × 20 = 0 × 8 + 0 × 4 + 0 × 2 + 1 × 1 = 1



0010 = 0 × 23 + 0 × 22 + 1 × 21 + 0 × 20 = 0 × 8 + 0 × 4 + 1 × 2 + 0 × 1 = 2



0011 = 0 × 23 + 0 × 22 + 1 × 21 + 1 × 20 = 0 × 8 + 0 × 4 + 1 × 2 + 1 × 1 = 3



If this is your first time working with different bases, you might have already figured out that the rightmost digit is multiplied by 20 in the case of the binary (base-2) system and multiplied by 100 in the case of the decimal (base-10) system. Then, the next digit is multiplied by 21 in the base-2 system and by 101 in the base-10 system. And so forth till we reach the leftmost digit. It is easy, but requires careful attention not to miss any digit or misjudge its power.



As an exercise, we will convert four more binary numbers, 1100, 1101, 1110, and 1111, to the decimal system. Try to do this on a piece of paper before comparing your answers with the solutions below.



1100 = 1 × 23 + 1 × 22 + 0 × 21 + 0 × 20 = 1 × 8 + 1 × 4 + 0 × 2 + 0 × 1 = 8 + 4 + 0 + 0 = 12



1101 = 1 × 23 + 1 × 22 + 0 × 21 + 1 × 20 = 1 × 8 + 1 × 4 + 0 × 2 + 1 × 1 = 8 + 4 + 0 + 1 = 13



1110 = 1 × 23 + 1 × 22 + 1 × 21 + 0 × 20 = 1 × 8 + 1 × 4 + 1 × 2 + 0 × 1 = 8 + 4 + 2 + 0 = 14



1111 = 1 × 23 + 1 × 22 + 1 × 21 + 1 × 20 = 1 × 8 + 1 × 4 + 1 × 2 + 1 × 1 = 8 + 4 + 2 + 1 = 15



Having come this far, it is time to revisit the hexadecimal system.



Binary system represents two states, such as ON and OFF



Hexadecimal Numbers :-

\--------------------

In Task 2, we grouped every 4 bits into a single hexadecimal digit. As we’ve seen earlier, a hexadecimal digit ranges between 0 and F. By taking a closer look at the table below, you will notice that a hexadecimal digit ranges between 0 and 15 in the decimal system. To replace 10, 11, 12, 13, 14, and 15 each with a single letter/digit, A, B, C, D, E, and F are chosen. The table below is something you would encounter in any tutorial or chapter on the hexadecimal system.



|Decimal Number|Hexadecimal Digit|Binary Representation|
|-|-|-|
|0|0|0000|
|1|1|0001|
|2|2|0010|
|3|3|0011|
|4|4|0100|
|5|5|0101|
|6|6|0110|
|7|7|0111|
|8|8|1000|
|9|9|1001|
|10|A|1010|
|11|B|1011|
|12|C|1100|
|13|D|1101|
|14|E|1110|
|15|F|1111|



Optional :-

\---------

Converting From Hexadecimal to Decimal System.



This subsection is optional. If you are curious about converting a hexadecimal number to a decimal number, you would follow the same approach we used for binary conversion. Let’s say that we want to convert the hexadecimal number 9B DF to decimal.



9BDF = 9 × 163 + 11 × 162 + 13 × 161 + 15 × 160 = 9 × 4096 + 11 × 256 + 13 × 16 + 15 × 1 = 39,903



Octal Numbers :-

\--------------

The octal system refers to base 8. In other words, it uses the digits between 0 and 7. While the hexadecimal system uses base 16 and groups 4 bits, the octal system uses base 8 and groups 3 bits. The table below shows how the octal digits relate to their binary counterparts.



|Decimal Number|Octal Digit|Binary Representation|
|-|-|-|
|0|0|000|
|1|1|001|
|2|2|010|
|3|3|011|
|4|4|100|
|5|5|101|
|6|6|110|
|7|7|111|



Optional :-

\---------

Converting From Octal to Decimal System.



Converting an octal number to its decimal equivalent follows the steps of the previous conversions. Consider the octal number 357.



357 = 3 × 82 + 5 × 81 + 7 × 80 = 3 × 64 + 5 × 8 + 7 × 1 = 239



Lab :-

\----

Question 1 :-

\-----------

* Decimal Representation:

&#x20;  255

* Binary Representation:

&#x20;  1111 1111

* Octal Representation:

&#x20;  377

* Hexadecimal Representation:

&#x20;  FF



Question 2 :-

\-----------

* Decimal Representation:

&#x20;  171

* Binary Representation:

&#x20;  1010 1011

* Octal Representation:

&#x20;  253

* Hexadecimal Representation:

&#x20;  AB



Question 3 :-

\-----------

* Decimal Representation:

&#x20;  16,777,215

* Binary Representation:

&#x20;  1111 1111 1111 1111 1111 1111

* Octal Representation:

&#x20;  77,777,777

* Hexadecimal Representation:

&#x20;  FF FF FF



Answer the questions below:

What is the hexadecimal FF in binary?



Answer : 1111 1111

\-------



What is the hexadecimal AB in decimal?



Answer : 171

\------

Convert the hexadecimal FF FF FF to decimal. After you round up the decimal value to the nearest million, how many millions is that?



Answer : 17

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conclusion :-

\-----------

In this room, we covered several topics related to how numeric values are represented and stored in computer memory. We covered the following systems:



1. Decimal (Base-10) system :-

&#x20;  -------------------------

This is the system we use in our everyday life.



2\. Binary (Base-2) system :-

&#x20;  -----------------------

Computers understand two states, which are encoded as 0 and 1.



3\. Hexadecimal (Base-16) system :-

&#x20;  -----------------------------

Every 4 binary digits (bits) can be grouped as one hexadecimal digit. A hexadecimal digit ranges between 0 and F.



4\. Octal (Base-8) system :-

&#x20;  ----------------------

Every 3 binary digits (bits) can be grouped as one octal digit. An octal digit ranges between 0 and 7. This one is less commonly encountered on computer systems.

Moreover, we learned how a color can be represented.



We covered :-

\-----------



1. Bit :-

&#x20;  ----

It is short for binary digit, and it can be either 0 or 1.



2\. Byte :-

&#x20;  -----

On modern systems, a byte is 8 bits. It is also referred to as an octet.



3\. Hex color :-

&#x20;  ----------

A color is represented as a combination of red, green, and blue on computer systems. If one byte is assigned for each of the primary colors (red, green, and blue), we can get more than 16 million color combinations.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Data Encoding Room :-

\------------------

Task 1 :-

\-------

Introduction :-

\-------------

In the previous room, you learned how numbers are represented in the computer as binary digits (bits) and how these bits can be grouped into hexadecimal digits; we also explored how to express colors using numbers. Now, if everything is stored as numbers, how do we convert them to letters, punctuation, and emojis?



In this room, you will learn that characters are just numbers with agreed meanings. That agreement is called an encoding. Have you ever opened a document, visited a web page, or downloaded movie subtitle files only to see the file appear as weird gibberish? One reason for that is that the user who saved the file and the user who opened it are using different encodings.



Representation is the idea that data lives as bits and numbers in memory. At the same time, encoding is the specific, agreed-upon mapping between numbers and meanings, such as which number corresponds to the character “A”. In text, each character, like q, 5, or !, is assigned a numeric code, so a string becomes a sequence of numbers that the computer stores and moves around just like any other data.



Learning Objectives :-

\--------------------

Upon completion of this room, you will learn about:



* ASCII
* Unicode
* UTF-8, UTF-16, and UTF-32
* How emoji is encoded And what causes weird gibberish characters

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

ASCII :-

\------

We already learned that digital computers only understand zeroes and ones. Starting from 0 and 1, how can we save and display text? For example, how can we save the text “TryHackMe” in a file? What will such a file contain?



To be able to answer this, we need to agree on what bits represent T, what bits represent r, what bits represent y, and so on. Let’s say that we all agree to represent T with the following stream of bits: 01010100. Then all computer systems should store T the same way, and later, when a computer encounters 01010100, it will recognize it as T. Of course, we need to do this for all letters in the alphabet, digits, and special characters. This approach requires a standard that computer manufacturers, designers, and programmers agree to adhere to. One of the earliest standards for English letters was ASCII.



ASCII stands for American Standard Code for Information Interchange, and it is an early character encoding from 1963 that uses numbers 0-127 to represent English letters, digits, punctuation, and some control characters. Remember that A stands for American, as this will come in handy later. As you might have noticed, the original ASCII was limited to seven bits. ASCII acts as a small bilingual dictionary between text and numeric codes. Consider the following samples from the original ASCII table. Since the table has 128 entries, we only made a brief selection to give you an idea of how things are represented in ASCII.



|Decimal|Hexadecimal|Binary|Symbol|Description|
|-|-|-|-|-|
|...|...|...|...|...|
|48|30|00110000|0|Zero|
|...|...|...|...|...|
|57|39|00111001|9|Nine|
|...|...|...|...|...|
|65|41|01000001|A|Uppercase A|
|...|...|...|...|...|
|88|58|01011000|X|Uppercase X|
|89|59|01011001|Y|Uppercase Y|
|90|5A|01011010|Z|Uppercase Z|
|91|5B|01011011|\[|Opening bracket|
|92|5C|01011100|\|Backslash||
|93|5D|01011101|]|Closing bracket|
|94|5E|01011110|^|Caret - circumflex|
|95|5F|01011111|\_|Underscore|
|96|60|01100000|`|Grave accent|
|97|61|01100001|a|Lowercase a|
|98|62|01100010|b|Lowercase b|
|99|63|01100011|c|Lowercase c|
|...|...|...|...|...|
|122|7A|01111010|z|Lowercase z|
|...|...|...|...|...|
|127|7F|01111111|DEL|Delete|



There are several things that you can observe.



* First, letters are in order. If you know the hexadecimal or decimal number for b, you can figure out the decimal number of a, c, and later lower-case letters. For example, a, b, and c are assigned the hexadecimal numbers 61, 62, and 63, respectively. Same for upper-case letters A to Z and digits 0 to 9. When using ASCII encoding, a computer system reads 41 in a file and displays A on the screen; when it reads 42, it displays B, and so on.



* Secondly, each character has its own ASCII, for example, \[ is represented by the hexadecimal number 5B.



“TryHackMe” in ASCII :-

\---------------------

Let’s say you open a text file, write “TryHackMe” and save it as file.txt. How will the file look on the bit level? Let’s find out.



If you are interested in seeing the storage on the disk, bit by bit, and assuming that it is using ASCII, you will see something similar to the following:



01010100 01110010 01111001 01001000 01100001 01100011 01101011 01001101 01100101 00001010



Obviously, this is not readable by any human being. These are the exact binary representations of all the letters in “TryHackMe” followed by a new line. When you open this file, your editor will read these bits and display the following characters: T r y H a c k M e \\n; the \\n is a new line that you get when you hit the Enter key.



Because reading binary numbers is cumbersome and error-prone for us, we prefer to use hexadecimal digits. As you remember from the previous room, we group 4 bits into a single hexadecimal digit. Our file looks like this in hexadecimal: 54 72 79 48 61 63 6b 4d 65 0a



And if you want to look up the decimal representation, it would be as follows: 124 162 171 110 141 143 153 115 145 012; however, it is uncommon to use decimal digits. It is more common to use hexadecimal digits when we want to show the bits.



You can use the attached static site yourself to experiment more.



European Languages :-

\-------------------

ASCII provided a way to encode the English alphabet; however, we need an encoding to support other European languages such as Spanish (ñ, ¿), German (ß, ü), Polish (ł, ń), Czech (č, ř), and Romanian (ș, ț), to name a few. ASCII uses 7 bits, and with an eighth bit, we get 128 more characters to cover. However, the reality is more challenging; the additional 128 characters are not enough to cover all the letters of the European languages. The ISO/IEC 8859 Series (International Standards) created several standards; each standard covered a set of languages:



1. ISO-8859-1 (Latin-1): Covered Western European languages like German (ß, ü), French (é, ç), Spanish (ñ, ¿), Italian, Portuguese, Catalan, and Nordic languages (e.g., Icelandic ð/Ð). Check this link(opens in new tab).



2\. ISO-8859-2 (Latin-2): Supported Central/Eastern European languages like Polish (ł, ń), Czech (č, ř), Hungarian (ő, ű), Croatian (đ), Romanian (ș, ț), and Slovak. Check this link(opens in new tab).



In other words, if your document is saved using ISO-8859-1 and later read and displayed as if it were saved using ISO-8859-2, non-English letters are likely to be displayed differently.



Lab :-

\----

Question 1 :-

\-----------

ASCII Character Encoder:

@

Decimal:

64

Hexadecimal:

40

Octal:

100

Binary:

01000000

ASCII Name:

At sign



Question 2 :-

\-----------

ASCII Character Encoder:

\#

Decimal:

35

Hexadecimal:
23

Octal:
43

Binary:

00100011

ASCII Name:

Number sign



Question 3 :-

\-----------

and question number three answer will be BEL



Answer the questions below:

What is the ASCII code in decimal for the character @?



Answer : 64

\------



What is the character that has the ASCII code of 35 in decimal?



Answer : #

\------



What is the name of the character that has the ASCII code of 7?



Answer : BEL

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Unicode :-

\--------

We learned that ASCII is a 7-bit standard that defines 128 characters covering English letters, digits, and basic punctuation. We also noticed how ASCII, with its seven bits, didn’t have room for characters such as ñ, €, あ, or ب. Using eight bits, extended ASCII tried patching this with regional variants (ISO-8859-1, ISO-8859-2, Windows-1252, among many others), but this caused chaos! For example, if the sender writes and saves Ø using ISO 8859-1 (Latin 1) encoding and the recipient opens and reads the document using ISO 8859-2 (Latin 2) encoding, they will see Ř. Hence, it is clear how opening a document requires us to use the same encoding used when saving it; otherwise, various characters will not be displayed correctly, or even more confusingly, they might be incorrectly replaced.



Unlike English, which has 26 letters and needs 52 characters to cover upper-case and lower-case letters, Arabic needs more than 250 characters to cover its various ligatures and diacritics. Moreover, the number escalates rapidly when considering Japanese and Chinese. In Japanese, 2,136 Kanji (logographic characters) are considered daily-use characters, as mandated by Japan’s Ministry of Education. In fact, the JIS X 0208 standard defines 6,879 characters. In Chinese, educated natives recognize around 8,000 characters. Furthermore, the GB 18030-2022 defines more than 87,887 Hanzi (Chinese characters). And still, we have not considered encoding emoticons (emoji).



In other words, it is essential for both the sender and the recipient to use the same encoding; moreover, we need an encoding that can include all the characters from all languages. This situation brings us to Unicode.



Unicode is a universal character encoding standard. It assigns unique code points to characters from all modern and historical writing systems worldwide. Unicode supports the interchange, processing, and display of text in diverse languages. In other words, we don’t need to worry about picking a specific encoding standard that is compatible with the language we are using. Furthermore, this makes it easy to use different languages in a single file or message. And most importantly, because this is a standard that fits all, we don’t need to worry about the encoding used by the original author, as they will also be using Unicode.



Unicode is a character set standard that assigns a unique number to every character across all languages. Examples:



U+0041 = Latin “A”

U+03A9 = Greek “Ω”

U+3042 = Japanese Hiragana “あ”

Unicode 17.0 is currently the latest version of the Unicode(opens in new tab) Standard. It defines close to 157 thousand characters, almost 4,000 of them are emoji sequences.



UTF-8, UTF-16, and UTF-32

Because you will encounter UTF-8, UTF-16, and UTF-32, we will briefly cover them without going into too much depth. What you need to know is that UTF-8 is very common on the modern web. It encodes Unicode points into 1 to 4 bytes dynamically. In other words, it decides on the number of bytes based on the character complexity. ASCII characters (U+0000 to U+007F) use exactly 1 byte, identical to the original ASCII, ensuring seamless backward compatibility. Non-ASCII characters like Ω (U+03A9) use 2 bytes, while complex scripts or emoji like 🔥 (U+1F525) require 4 bytes. This flexibility allows us to cover the Unicode standard without wasting bytes.



UTF-16 takes a different path; it uses either 2 or 4 bytes per character. Common characters, like most Latin, Cyrillic, or Chinese Hanzi, fit in 2 bytes; however, rarer ones, like emoji or ancient scripts, require a pair, i.e., two 16-bit units totaling 4 bytes. For example, the letter A is encoded as U+0041, while the emoji 🔥 needs two and is encoded as U+D83D U+DD25.



Finally, UTF-32 is the simplest but also the most wasteful; every Unicode code point uses exactly 4 bytes. For example, A is encoded as U+00000041 and 🔥 is encoded as U+0001F525.



Let’s explore a few more examples:



* 龍 : One of the Chinese characters that appear on offensive Linux distributions, such as Kali, is “龍”, which means “dragon”. In Unicode, it is U+9F8D or U+00009F8D, depending on whether it is UTF-16 or UTF-32.
* 😊: This smiley face is nothing more than U+0001F60A in UTF-32 for a computer; that’s literally 0000 0000 0000 0001 1111 0110 0000 1010.
* ツ: The Japanese letter “tsu” which some people use as a smiley face in some regions outside Japan; it has the code U+30C4 or U+000030C4 depending on whether it is UTF-16 or UTF-32.
* ت : is the Arabic letter “taa,” and some people use it as a smiley outside the Arab world; it looks close enough to a smiley face. From a Unicode perspective, that’s U+062A.
* ♞: The black knight in chess uses the Unicode U+265E; in other words, the computer reads 0010 0110 0101 1110 and shows you a black knight, thanks to Unicode.

We have created a static site to help you look up characters and explore new ones available in most standard fonts.



Lab :-

\----

Question 1 :-

\----------

1. so here we first copy 😌 and paste like that and values we get UTF-32 value.

Unicode Character Encoder:

😌

UTF-8:

0xF0 0x9F 0x98 0x8C

UTF-16:

U+D83D U+DE0C

UTF-32:

U+0001F60C

Decimal:

128524

Hexadecimal:

00 01 F6 0C

Binary:

0000 0000 0000 0001 1111 0110 0000 1100



Question 2 :-

\-----------

Here we give that シand we get the UTF-16 value.

Unicode Character Encoder:

シ

UTF-8:

0xE3 0x82 0xB7

UTF-16:

U+30B7

UTF-32:

U+000030B7

Decimal:

12471

Binary:

0000 0000 0000 0000 0011 0000 1011 0111

Unicode Name:

UNICODE CHARACTER U+000030B7



Question 3 :-

\----------

Here we give that UTF-16 value U+2615 and we get that ☕ in unicode character encoder.

Unicode Character Encoder:

☕

UTF-8:

0xE2 0x98 0x95

UTF-16:

U+2615

UTF-32:

U+00002615

Decimal:

9749

Hexadecimal:

00 00 26 15

Binary:

0000 0000 0000 0000 0010 0110 0001 0101

Unicode Name:

UNICODE CHARACTER U+00002615



Question 4 :-

\-----------

Here we give that UTF-16 value U+2658 and we get that ♘ in unicode character encoder.

Unicode Character Encoder:

♘

UTF-8:

0xE2 0x99 0x98

UTF-16:

U+2658

UTF-32:

U+00002658

Decimal:

9816

Hexadecimal:

00 00 26 58

Binary:

0000 0000 0000 0000 0010 0110 0101 1000

Unicode Name:

UNICODE CHARACTER U+00002658



Answer the questions below:

1. What is the UTF-32 encoding of 😌?



Answer : U+0001F60C



What is the UTF-16 encoding of シ? Note that ツ and シ are two different characters.



Answer : U+30B7



What is the character that has the following UTF-16 encoding U+2615?



Answer : ☕



What is the character that has the following UTF-16 encoding U+2658?



Answer : ♘



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

* Conclusion :-

\-----------

In this room, we learned about ASCII and its limitations, and about Unicode and three encoding standards: UTF-8, UTF-16, and UTF-32. We explored how Unicode enables us to cover not only the world’s languages but also symbols such as chess pieces and emojis.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Python: Simple Demo Room :-

\-------------------------

Task 1 :-

\------

Introduction :-

\-------------

In the first two rooms, Data Representation and Data Encoding, we learned how computers understand numbers, characters, colors, and even emojis. In this room, we will explore one of the most popular and friendly programming languages, Python.



You may have heard of the Python programming language numerous times. Python is a high-level general-purpose programming language. By high-level, we mean it hides most implementation details; general-purpose means you can use Python for a wide variety of scenarios, from web applications and automation scripts to data science and machine learning.



In this room, we will create a “Guess the Number” game. Our plan will be as follows:



* The computer secretly picks a number between 1 and 20.
* The user keeps guessing until they get it right.
* The computer tells the user whether their guess is too low or too high.
* An example session running the program is shown below:





Terminal:

\---------

ubuntu@tryhackme:\~$ python guess\_the\_number.py

I'm thinking of a number between 1 and 20

Take a guess: 10

Too high, try again.

Take a guess: 5

Too low, try again.

Take a guess: 7

Too low, try again.

Take a guess: 8

You got it in 4 tries!



Learning Objectives :-

\--------------------

* Learn about Python variables
* Understand how conditional statements are used
* See iteration (loop) in action

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Variables :-

\---------

The program needs to start by picking a random secret number between 1 and 20. Then the user will begin making a guess after another till they get it right. This approach requires two variables: secret and guess. We can also track the number of tries (attempts) it took the user to find the number; for this, we will use the variable tries.



Python offers the random.randint() method, which returns a random integer within the specified bounds. For example, random.randint(1, 20) returns a random number between 1 and 20. Since the user has not made any attempts, we set tries to 0; moreover, we set guess to a value outside the valid range. To tell the user that the program picked a number, we use Python’s print() method to display an informational message on the screen. We show the current Python script below:



\-----------------------------------------------------------------------------------

import random  # gives us tools for picking random numbers



secret = random.randint(1, 20)  # a <= secret <= b

tries = 0

guess = 0  # start with a value that cannot be the secret (since secret is 1..20)



print("I'm thinking of a number between 1 and 20")

\------------------------------------------------------------------------------------

This code snippet achieves the following:



* Use the random.randint() method from the random library to pick a random number between 1 and 20 and save it to secret.
* Creates two variables, tries and guess, and sets them to 0.
* Display a message on the screen to inform the user that a number has been picked.
* With our variables ready, we prompt the user to make a guess and set guess accordingly. We begin by saving the user’s input to a temporary text variable, then use Python’s int() to convert it to an integer. Furthermore, we need to increment tries each time the user makes a guess.



\------------------------------------------------------------------

text = input("Take a guess: ")  # input() returns text (a string)

guess = int(text)  # convert the text to a number



tries = tries + 1  # add 1 try (written long-form for clarity)

\------------------------------------------------------------------

So far, our program does the following:



* Pick a random number between 1 and 20 and save it in secret.
* Ask the user to take a guess, convert it to an integer, and save it in guess.
* Increment tries by 1.
* To check whether the user made a correct guess, we should be able to compare against various cases; this requires conditional statements and comparison operators.

\----------------------------------------------------------------------------------

import random  # gives us tools for picking random numbers



secret = random.randint(1, 20)  # a <= secret <= b

tries = 0

guess = 0  # start with a value that cannot be the secret (since secret is 1..20)



print("I'm thinking of a number between 1 and 20")



text = input("Take a guess: ")  # input() returns text (a string)

guess = int(text)  # convert the text to a number



tries = tries + 1  # add 1 try

\-----------------------------------------------------------------------------------



Answer the questions below:

1. What is the name of the function we used to display text on the screen?



Answer: print()

\------

2\. What is the name of the function that we used to convert user input to an integer?



Answer : int()

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Conditional Statements :-

\----------------------



Download Task Files

Before starting, please note that you can download the attached zip file. It includes all versions of the program that are present on the target VM. This archive allows you to review the project's evolution, compare implementations, or test each version independently on your local machine. Having all iterations in one package should make your work more efficient.



Next, we compare the user’s guess to the secret number and give a helpful hint: whether it is out of range, too low, too high, or if they got it right. It is like asking ourselves, “Is the number less than 1 or greater than 20?” If the answer is yes, we tell the user that the number is out of range. If the answer is no, we pose a second question: “Is the user’s guess less than the secret number?” If the answer is yes, we tell the user that the guess is too low. Let’s rephrase this in pseudo-code, i.e., English language that is closer to the programming language.



* If the guess is less than 1 or greater than 20, print “Out of range.” (If this is not the case, proceed to the next step.)
* Else if the guess is less than the secret number, print “Too low.” (If this is not the case, proceed to the next step.)
* Else if the guess is larger than the secret number, print “Too high.” (If this is not the case, proceed to the next step.)
* Else print “You got it.”



By reflecting on the above steps, it is only logical that if the guess is not less than or larger than the secret number, it would be equal to the secret number. In programming, whenever the condition after the “if” is not true (written as if CONDITION: in Python), the program checks the condition after the “else if” (written as elif CONDITION: in Python), and if it is also false, it checks the next “else if”. If there are no more “else if” statements left, the program executes the final “else” (written as else: in Python). Let’s convert the above pseudo-code to working Python code.



\--------------------------------------------------------

\# Give a hint using if / elif / else.

if guess < 1 or guess > 20:

&#x20;   print("That number is out of range. Try again.")

elif guess < secret:

&#x20;   print("Too low, try again.")

elif guess > secret:

&#x20;   print("Too high, try again.")

else:

&#x20;   print("You got it in", tries, "tries!")

\---------------------------------------------------------



In this implementation, comparing the user’s guess to the chosen secret will lead to various cases:



* The user makes a guess outside the allowed bounds, i.e., 1 and 20
* The user’s guess is less than secret
* The user’s guess is greater than secret
* The user’s guess is correct



If the above looks confusing, consider the following numerical examples.



Numerical Example 1 :-

\-------------------



We assume that the secret number is 10. If the user inputs 30, the first if condition will evaluate to true, and Python will execute the part after if guess < 1 or guess > 20: and print “That number is out of range. Try again.”



Numerical Example 2 :-

\--------------------



We assume that the secret number is 10. Suppose the user inputs 5, the first if condition will evaluate to false because 5 is neither less than 1 nor greater than 20. Python will check the condition following the first elif and it will evaluate to true because 5 is indeed less than 10. Consequently, the program will print “Too low, try again.”



Numerical Example 3 :-

\--------------------



We assume that the secret number is 10. Suppose the user inputs 15, the first if condition will evaluate to false because 15 is neither less than 1 nor greater than 20. The program will check the condition following the first elif and it will also evaluate to false because 15 is not less than 10. The program will check the condition following the second elif, and this one will evaluate to true, because 15 is larger than 10. As a result, the program will display, “Too high, try again.”



The First Draft :-

\----------------

In this task, we built a working program that you can test for yourself and edit in the attached VM. The main limitation is that this program gives the user one chance. In the next task, we upgrade this program to allow the user an infinite number of tries to make the correct guess. The program below is saved as guess\_v2.py in the /home/ubuntu/Python-Demo directory.



\----------------------------------------------------------------------------------

import random  # gives us tools for picking random numbers



secret = random.randint(1, 20)  # a <= secret <= b

tries = 0

guess = 0  # start with a value that cannot be the secret (since secret is 1..20)



print("I'm thinking of a number between 1 and 20")



text = input("Take a guess: ")  # input() returns text (a string)

guess = int(text)  # convert the text to a number



tries = tries + 1  # add 1 try



\# Give a hint using if / elif / else.

if guess < 1 or guess > 20:

&#x20;   print("That number is out of range. Try again.")

elif guess < secret:

&#x20;   print("Too low, try again.")

elif guess > secret:

&#x20;   print("Too high, try again.")

else:

&#x20;   print("You got it in", tries, "tries!")

\----------------------------------------------------------------------------------

Answer the questions below:

1. How does Python write “else if”?



Answer : elif

\-------

2\. What will the program display if the user’s input is 50?



Answer : That number is out of range. Try again.

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Iterations :-

\-----------

It is too hard to guess the number when given a single chance. To make this game more interesting, it should provide the user with at least a few chances. We will be highly tolerant and allow the user as many attempts as needed to find the secret number. To give the user more than one chance, we need to use our secret weapon: loops! In programming, loops, or more formally, iterations, allow us to execute the same lines of code multiple times. In more formal phrasing, we can iterate over the same code block as long as a specific condition holds.



Let’s look at a few examples of iteration in our daily lives. Consider the case where you want to buy a new t-shirt: you will see one shop after another until you find one that suits you. The condition here is finding a suitable t-shirt. Consider another example where you are searching for an empty parking space in a vast parking lot. You will check one row of cars after another until you finally find a space. The condition here is finding a suitable parking space.



Back to our game, we will keep repeating the code we wrote in Task 3 until the user’s guess matches the secret number. In Python, “does not equal” is written as !=. In other words, the condition “guess does not equal secret” is written as guess != secret. To write this as a while loop, we use the form while CONDITION:; in our case, it is while guess != secret:.



Let’s paste the code from Task 3 in the body of our while loop.



\-----------------------------------------------------------------------

\# Repeat until the user guesses the secret number.

while guess != secret:

&#x20;   text = input("Take a guess: ")  # input() returns text (a string)

&#x20;   guess = int(text)  # convert the text to a number

&#x20;

&#x20;   tries = tries + 1  # add 1 try



&#x20;   # Give a hint using if / elif / else.

&#x20;   if guess < 1 or guess > 20:

&#x20;       print("That number is out of range. Try again.")

&#x20;   elif guess < secret:

&#x20;       print("Too low, try again.")

&#x20;   elif guess > secret:

&#x20;       print("Too high, try again.")

&#x20;   else:

&#x20;       print("You got it in", tries, "tries!")

\------------------------------------------------------------------------

The code above will execute as follows. First, Python will check the condition after the while; if it is true, it will run all the indented lines. If the condition is false, it terminates.



Numerical Example 1 :-

\-------------------



We assume that the secret number is 10. In the first run, the guess is 0. The while condition will evaluate to true because 10 is not equal to 0. The program will ask the user to “Take a guess,” and it will proceed from there.



Numerical Example 2 :-

\-------------------



We assume that the secret number is 10. If the user entered 5 earlier, it means they did not guess the number in the previous attempt. The while condition will evaluate to true because 10 is not equal to 5. The program will give the user another chance and prompt them to “Take a guess.”



Numerical Example 3 :-

\--------------------



We assume that the secret number is 10. If the user entered 10 earlier, it means they successfully guessed the number in the previous attempt. Let’s see if the program will prompt them for another guess. The while loop will evaluate to false because 10 is equal to 10; in other words, 10 != 10 is false. The indented code block within the while statement will no longer execute.



The Second Draft :-

\----------------

In this task, we have completed coding our game. You can test it for yourself and edit in the attached VM. The program below is saved as guess\_v3.py in the /home/ubuntu/Python-Demo directory.



\-----------------------------------------------------------------------------------

import random  # gives us tools for picking random numbers



\# ----------------------------

\# Guess the Number (Beginner Demo)

\# ----------------------------

\# The computer picks a secret number.

\# The player keeps guessing until they find it.



secret = random.randint(1, 20)  # a <= secret <= b

tries = 0

guess = 0  # start with a value that cannot be the secret (since secret is 1..20)



print("I'm thinking of a number between 1 and 20")



\# Repeat until the user guesses the secret number.

while guess != secret:

&#x20;   text = input("Take a guess: ")  # input() returns text (a string)

&#x20;   guess = int(text)  # convert the text to a number

&#x20;

&#x20;   tries = tries + 1  # add 1 try



&#x20;   # Give a hint using if / elif / else.

&#x20;   if guess < 1 or guess > 20:

&#x20;       print("That number is out of range. Try again.")

&#x20;   elif guess < secret:

&#x20;       print("Too low, try again.")

&#x20;   elif guess > secret:

&#x20;       print("Too high, try again.")

&#x20;   else:

&#x20;       print("You got it in", tries, "tries!")

\---------------------------------------------------------------------------------------



Answer the questions below:

What type of loop does this program use?



Answer : while

\-------

What will the program display if the user makes the correct guess in 3 tries?



Answer : You got it in 3 tries!

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\-------

Conclusion :-

\-----------

In this room, we covered three key pillars in imperative programming languages:



* Variables
* Conditionals with if and else
* Loops with while

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



JavaScript: Simple Demo Room :-

\-----------------------------

Task 1 :-

\------

Introduction :-

\-------------

The purpose of this room is to give you an idea about one popular programming language: JavaScript. It is almost certain that you have come across the name JavaScript; however, throughout this room, we assume that you have never studied or written programs in this language.



JavaScript is used in most of the web pages that you visit on a day-to-day basis. Consequently, when we think of JavaScript engines, web browsers come to mind. In fact, JavaScript was initially developed to run on client machines, in particular, within a web browser. However, this has changed with the release of Node.js, which enables developers to build web applications with JavaScript. Consequently, as Node.js spread, JavaScript was no longer just a client-side programming language but also a server-side one.



In this room, we will create a “Guess the Number” game. Our plan will be as follows:



* The computer secretly picks a number between 1 and 20.
* The user keeps guessing until they get it right.
* The computer tells the user whether their guess is too low or too high.
* An example session running the program is shown below.





Terminal

\--------

ubuntu@tryhackme:\~/JavaScript-Demo$ node guess\_v3.js

I'm thinking of a number between 1 and 20

Take a guess: 10

Too high, try again.

Take a guess: 5

Too low, try again.

Take a guess: 7

You got it in 3 tries!



We will try to follow an approach similar to the one we followed in the Python: Simple Demo room. Hence, we chose the same idea to implement. The reason for this is to allow you to explore the main language differences for the same program idea.



Learning Objectives :-

\--------------------

* Learn about JavaScript variables
* Understand how conditional statements are used
* See iteration (loop) in action

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Variables :-

\----------

You can follow along by starting the attached VM by clicking the Start Lab Machine button shown above. Visual Studio Code should open automatically as shown in the screenshot below.



JavaScript demo opened



Setting the Stage :-

\------------------

Before starting, we should point out that JavaScript files can be executed in various ways; one way is to use your web browser, and another way is to use Node.js. However, for our purposes, the easiest way to get started is by using Node.js(opens in new tab). It is easy to download for your system and run your JavaScript files from the command line.



If you are curious about running JavaScript in your web browser, it is pretty simple. In your favorite web browser, access the Web Developer Tools. For example, I need to press F12 in Firefox to open the console, where I can run my JavaScript code. A screenshot of a web browser running JavaScript code is shown below.



Running JavaScript code within a web browser



Note that in this room, we will test our JavaScript code exclusively using Node.js. This process can be run by typing node demo.js at the command line, where demo.js is the name of our JavaScript file.



Creating Variables :-

\-------------------

Going back to our “game”, we need to start by declaring variables. We think of a variable as a space in memory that stores a value and allows us to change this value later. For example, we want to keep track of the number of tries (attempts) a user has made, as well as the user’s guess. We can do this by declaring these two variables:



\--------------

let tries = 0;

let guess = 0;

\--------------

The let indicates that we are declaring variables. When the user starts, they have not made any attempts, so tries is set to 0; moreover, we initialize guess to a value that cannot accidentally be the secret number that the user is trying to guess. (On a side note secret is constant and will be covered in the next subsection.) Remember that the secret number is between 1 and 20.



Creating Constants :-

\-------------------

We use let to declare variables, whose value can change throughout the program; however, we use const to declare constants, whose value cannot change throughout the program.



The secret holds the number that we will try to find by guessing, and it should not change. As already mentioned, to declare a constant, we use the keyword const, for example, const secret = 12. To ensure that secret gets a new random value each time we run the program, we need to use JavaScript’s Math.random() method.

\-----------------------------------------------------------------------------------------------------------------------------------------

const secret = Math.floor(Math.random() \* (20)) + 1;

Although the details of this expression are not the key purpose of this room, we will share a brief breakdown for the curious readers.



Math.random() gives a random decimal between 0 (inclusive) and 1 (not including 1). Example: 0.372.

\* 20 stretches that range from 0 to (almost) 20. Example: 7.44.

Math.floor() removes the decimal by rounding down. Example: 7.44 becomes 7.

\+ 1 shifts the range from 0–19 to 1–20.

As a result, secret ends up being 1, 2, 3, …, up to 20.

\------------------------------------------------------------------------------------------------------------------------------------------



Displaying Output :-

\------------------

Once the secret number is picked, the program should inform the user that this step is complete. To display on the screen, console.log() can be used. In the example expression below, the string included between the double quotes will be displayed on screen.

\----------------------------------------------------------

console.log("I'm thinking of a number between 1 and 20");

\----------------------------------------------------------



Answer the questions below:

What word is used to declare a variable?



Answer : let

\-------



What word is used to declare a constant?



Answer : const

\-------



What is the method that we call to display text on the screen?



Answer : console.log()

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Prompting the User for Input :-

\-----------------------------



Download Task Files :-

\-------------------

Before starting, please note that you can download the attached zip file. It includes all versions of the program that are present on the target VM. This archive allows you to review the project's evolution, compare implementations, or test each version independently on your local machine. Having all iterations in one package should make your work more efficient.



In the previous task, we set our variables and constants; moreover, we picked a random secret number for the user to guess. Now, we need to prompt the user to take a guess and enter a number. In the first line, we wait for the user to input a value and save it in text. In the second line, we parse the text as an integer of base 10 using parseInt(text, 10). The parseInt() method takes the user input and converts it from text into an integer value.



\----------------------------------------------------

const text = await rl.question("Take a guess: ");

guess = parseInt(text, 10);

\-----------------------------------------------------



Optional Notes :-

\---------------



The await instruction pauses the system until the user responds. Obviously, Node.js’s default behavior is not to wait for a user to enter a value. Remember that Node.js is built as a runtime environment for web applications, not to run such a command-line JavaScript program. Consequently, we need to use libraries to override the default behavior and force Node.js to wait for the user. The following lines achieve this:



\----------------------------------------------------------------

import \* as readline from "node:readline/promises";

import { stdin as input, stdout as output } from "node:process";



const rl = readline.createInterface({ input, output });

\----------------------------------------------------------------



The first line borrows (import) the readline module so that the program can ask questions and wait for typed answers. The /promises part means it can “pause” neatly until the user responds. The second line imports two more modules, stdin, short for standard input (usually the keyboard), and stdout, short for standard output (usually the screen); moreover, it renames them to input and output respectively. The third line sets up the conversation channel using the “microphone” from line 1 and the “wires” from line 2.



Why is this so complicated to get command-line input? Because we are using Node.js to test our JavaScript program, we do not need to keep the server busy waiting for user input. Deviating from the expected default requires us to add these extra library imports.



Clean Execution :-

\---------------

To read user input, we had to create an interface we likened to a microphone. Before the program finishes, we need to close this interface. You would also switch off your microphone after the Q\&A session. To close the interface, we use rl.close(). As a result, our code will declare and initialize the rl (short for readline), use it to get text input from the user, and close() it. These three steps are shown below.



\------------------------------------------------------------------------------------------------

const rl = readline.createInterface({ input, output });



try {

//...

&#x20;   const text = await rl.question("Take a guess: "); // rl.question() returns text (a string)

//...

} finally {

&#x20;   rl.close();

}

\--------------------------------------------------------------------------------------------------



The try block creates a safe environment so that if something goes wrong, the program won’t crash. Think of it as trying to run a set of statements, and if something happens, handle it gracefully, and finally clean up.



Let’s summarize what we are doing:



* We are importing the readline module with the /promises part, indicating that the script will handle waiting without freezing everything
* Then we imported stdout (standard output) and stdin (standard input) as input and output
* Using these imported modules, we create the readline const with the name rl.
* The program makes its guess using Math.random() and saves that as secret, a constant.
* We declared two variables, tries and guess
* We displayed on the screen that “a number between 1 and 20” has been selected
* The user’s response is considered a guess and will be saved in text, a constant
* The user’s response is converted to a number using parseInt()
* The number of tries increases by one
* Finally, we clean up and close the readline interface, rl, that we created earlier

&#x20;



Putting it All Together :-

\------------------------

The first draft we have built so far is listed below and is also available on the system as guess\_v1.js, which can be found in the /home/ubuntu/JavaScript-Demo directory.

\-----------------------------------------------------------------------------------------------

import \* as readline from "node:readline/promises";

import { stdin as input, stdout as output } from "node:process";



const rl = readline.createInterface({ input, output });



try {

&#x20;   const secret = Math.floor(Math.random() \* (20)) + 1; // 1 <= secret <= 20

&#x20;   let tries = 0;

&#x20;   let guess = 0; // start with a value that cannot be the secret (since secret is 1..20)



&#x20;   console.log("I'm thinking of a number between 1 and 20");



&#x20;   const text = await rl.question("Take a guess: "); // rl.question() returns text (a string)

&#x20;   guess = parseInt(text, 10); // convert the text to a number



&#x20;   tries = tries + 1; // add 1 try



} finally {

&#x20;   rl.close();

}

\--------------------------------------------------------------------------------------------------



What’s Missing?

The most glaring missing component is that the user receives no feedback, even if they get the correct answer. Let’s get this implemented in the next task.



Answer the questions below:

1. What method is used to convert user input into a number?



Answer : parseInt()



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conditional Statements :-

\-----------------------

So far, you are playing the “guess the number” game, and the current program has no way to provide feedback on your choices. It asks you to make a guess, and it goes silent! Let’s make things more engaging and advance our program so it can evaluate user input and provide feedback.



We will follow the following logic steps:



* If it is outside the valid range, i.e., not between 1 and 20, we tell the user that their “number is out of range”
* If it is less than the secret number, we inform the user that it is “too low”
* If it is greater than secret, we inform the user that it is “too high”
* If it is not greater than and not less than the secret number, this means that it is equal to the secret number, and the user has successfully guessed it



From the above comparisons, you can see that if the first condition holds, there is no point in checking the second condition. Moreover, if the second condition holds and it is less than secret, there is no point in checking the third condition. Because the conditions are mutually exclusive, we can make use of else. We will present the conditions using JavaScript and discuss them afterwards.



\---------------------------------------------------------------

// Give a hint using if / else if / else.

if (guess < 1 || guess > 20) {

&#x20;   console.log("That number is out of range. Try again.");

} else if (guess < secret) {

&#x20;   console.log("Too low, try again.");

} else if (guess > secret) {

&#x20;   console.log("Too high, try again.");

} else {

&#x20;   console.log("You got it in", tries, "tries!");

}

\----------------------------------------------------------------



The above if, else if, and else statements will execute as follows:



1. if (guess < 1 || guess > 20) :-

&#x20;  ----------------------------

If the guess is less than 1 or the guess is greater than 20, then use console.log() to tell the user that the “number is out of range”. Note that || represents "or" in JavaScript.

2\. else if (guess < secret) :-

&#x20;  ------------------------

The else means that if the previous condition is not true, run this statement. if (guess < secret) will evaluate whether the guess is less than the secret. If this is the case, it will use console.log() to display “too low” on the screen

3\. else if (guess > secret):-

&#x20;  ------------------------

Similarly, the else will ensure that this statement won’t run unless the previous if has evaluated to false. Assuming that the last if condition evaluated to false, if (guess > secret) will assess its condition. In the case that guess is greater than secret, the console.log() displays “too high”



Finally, we see an else sitting by itself. This else means that if all previous if conditions are evaluated to false, the enclosed statement will execute. As we established earlier, if all previous conditions are evaluated to false, it means that the user guessed the number.

Putting it All Together Our draft can be updated to include the conditions we covered in this task. The previous draft will be expanded to provide the user with feedback on their guesses. The updated program we have constructed so far is listed below and is also available on the system as guess\_v2.js in the /home/ubuntu/JavaScript-Demo directory.



\---------------------------------------------------------------------------------------------

import \* as readline from "node:readline/promises";

import { stdin as input, stdout as output } from "node:process";



const rl = readline.createInterface({ input, output });



try {

&#x20;   const secret =

&#x20;       Math.floor(Math.random() \* (20)) + 1; // 1 <= secret <= 20

&#x20;   let tries = 0;

&#x20;   let guess = 0; // start with a value that cannot be the secret (since secret is 1..20)



&#x20;   console.log("I'm thinking of a number between 1 and 20");



&#x20;   const text = await rl.question("Take a guess: "); // rl.question() returns text (a string)

&#x20;   guess = parseInt(text, 10); // convert the text to a number

\-

&#x20;   tries = tries + 1; // add 1 try



&#x20;   // Give a hint using if / else if / else.

&#x20;   if (guess < 1 || guess > 20) {

&#x20;       console.log("That number is out of range. Try again.");

&#x20;   } else if (guess < secret) {

&#x20;       console.log("Too low, try again.");

&#x20;   } else if (guess > secret) {

&#x20;       console.log("Too high, try again.");

&#x20;   } else {

&#x20;       console.log("You got it in", tries, "tries!");

&#x20;   }

} finally {

&#x20;   rl.close();

}

\-------------------------------------------------------------------------------------------------



Let’s quickly review what this code does :-

\-----------------------------------------



* It picks a random secret number between 1 and 20
* It keeps track of the user’s guess and number of tries
* Then it asks the user to “Take a guess:”
* The user’s guess is received as text and converted to a number, and saved in guess
* We compare guess with secret and give feedback to the user about their attempt



Make sure that you have a good understanding of the script so far. You are not expected to write it yourself; however, you should be able to explain it by looking at it.



What’s Missing?

This code runs once, giving the user a single chance. This situation is shown in the interaction below.





Terminal

\--------

ubuntu@tryhackme:\~/JavaScript-Demo$ node guess\_v2.js

I'm thinking of a number between 1 and 20

Take a guess: 10

Too low, try again.



Obviously, that’s not a fun game if the user gets only one chance. We need to give the user more chances until they make the correct guess. In the next task, we will get our script to provide the user with many chances to make the game more fun.



Answer the questions below:

1. The secret is 10. What will our program display on the screen if the user makes a guess of 15?



Answer : Too high, try again.

\-------



2\. The secret is 10. What will our program display on the screen if the user makes a guess of 35?



Answer : That number is out of range. Try again.

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------



Task 5 :-

\-------

Iterations :-

\----------

The script we have so far efficiently provides feedback on the user’s guess; however, it does not give them a second chance. In this task, we will make the necessary changes so that it keeps prompting the user for new guesses until they figure it out.



One way to achieve this is to keep prompting the user to make new guesses as long as their guess is wrong, i.e., while their guess is not equal to secret. That’s quite easy to express in JavaScript: while (guess !== secret). The !== means “not equal”. This is called a while loop and is written as shown below:



\-----------------------------------------------------

// Repeat until the user guesses the secret number.

while (guess !== secret) {

&#x20;   // Loop body: instructions to be repeated

}

\-----------------------------------------------------



The next part to decide is what to include in the body of this while loop. Based on the program logic we have built so far, we should repeat the following:



* Prompt the user to take a guess
* Convert the user’s input to a number and save it in guess
* Increase the number of tries by one
* Check guess with respect to the lower and upper limits
* If it is within the limits, compare it to the secret number
* Display feedback to the user about their choice



And we will repeat if the users didn’t make the correct guess.



The JavaScript code with the while loop filled is shown below.



\---------------------------------------------------------------------------------------------------------

// Repeat until the user guesses the secret number.

while (guess !== secret) {

&#x20;   const text = await rl.question("Take a guess: "); // rl.question() returns text (a string)

&#x20;   guess = parseInt(text, 10); // convert the text to a number



&#x20;   tries = tries + 1; // add 1 try



&#x20;   // Give a hint using if / else if / else.

&#x20;   if (guess < 1 || guess > 20) {

&#x20;       console.log("That number is out of range. Try again.");

&#x20;   } else if (guess < secret) {

&#x20;       console.log("Too low, try again.");

&#x20;   } else if (guess > secret) {

&#x20;       console.log("Too high, try again.");

&#x20;   } else {

&#x20;       console.log("You got it in", tries, "tries!");

&#x20;   }

}

Putting it All Together

The program we have constructed so far is listed below and is also available on the system as guess\_v3.js.





import \* as readline from "node:readline/promises";

import { stdin as input, stdout as output } from "node:process";



const rl = readline.createInterface({ input, output });



try {

&#x20;   const secret =

&#x20;       Math.floor(Math.random() \* (20)) + 1; // 1 <= secret <= 20

&#x20;   let tries = 0;

&#x20;   let guess = 0; // start with a value that cannot be the secret (since secret is 1..20)



&#x20;   console.log("I'm thinking of a number between 1 and 20");



&#x20;   // Repeat until the user guesses the secret number.

&#x20;   while (guess !== secret) {

&#x20;       const text = await rl.question("Take a guess: "); // rl.question() returns text (a string)

&#x20;       guess = parseInt(text, 10); // convert the text to a number



&#x20;       tries = tries + 1; // add 1 try



&#x20;       // Give a hint using if / else if / else.

&#x20;       if (guess < 1 || guess > 20) {

&#x20;           console.log("That number is out of range. Try again.");

&#x20;       } else if (guess < secret) {

&#x20;           console.log("Too low, try again.");

&#x20;       } else if (guess > secret) {

&#x20;           console.log("Too high, try again.");

&#x20;       } else {

&#x20;           console.log("You got it in", tries, "tries!");

&#x20;       }

&#x20;   }

} finally {

&#x20;   rl.close();

}

\-----------------------------------------------------------------------------------------------------------------



You can test it on the system by running node guess\_v3.js; it can be found in /home/ubuntu/JavaScript-Demo. Every time you rerun the program, it should pick a new secret number for you to guess.



\-----------------------------------------------------

Terminal

\--------

ubuntu@tryhackme:\~/JavaScript-Demo$ node guess\_v3.js

I'm thinking of a number between 1 and 20

Take a guess: 10

Too low, try again.

Take a guess: 15

Too high, try again.

Take a guess: 13

Too low, try again.

Take a guess: 14

You got it in 4 tries!

\------------------------------------------------------

It should be noted that the file node guess\_v4.js, on the VM and in the zip file attached to Task 3, further improves this program. You are encouraged to take a look; however, it is not critical for this introductory room.



Answer the questions below:

1. What is the name of the loop that we used in this task?



Answer : while

\-------



2\. What is the name of the variable that is incremented by one when the user makes a new wrong guess?



Answer : tries

\-------



3\. How is “not equal” written in JavaScript?



Answer : !==

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 6 :-

\-------

Conclusion :-

\----------

In this room, we covered three key pillars in imperative programming languages:



* Variables
* Conditionals with if and else
* Loops with while



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Database SQL Basics Rooms :-

\--------------------------

Task 1 :-

\-------

Introduction :-

\-------------

How can a café keep track of every order and still quickly answer questions about them later?



A café notebook with handwritten drink orders and an arrow pointing to a laptop displaying the same data organized in a database table with Time, Drink, and Price columns



In the Computer Fundamentals module (coming soon), we have seen how computers can process information while running. But what happens when the computer is turned off? Where does the information go?

In this room, you will be helping a small business make sense of its data. As the company grows, keeping track of information using simple files becomes slow and confusing. Databases solve this problem by storing information in a structured way that is easy to search and manage.



Learning Objectives :-

\--------------------

* Understand what data is and why it matters
* Explain what a database is and why it is used
* Understand what SQL is and what it is used for
* Identify tables, rows, and columns
* Write simple SQL queries to retrieve information



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Understanding Tables, Rows, and Columns :-

\----------------------------------------

* In a café database table, what does one row represent?



* In this table, each column represents one type of information, such as a name or a price.



* Each row represents a complete record, and the table contains all records.



Imagine a small café.



At first, the café owner writes each order in a paper notebook to track orders and payments.



Each order includes :-

\--------------------



1. The drink name

2\. The price

3\. The time of the order



This works fine when the café is small. However, after many days, the notebook becomes full. Finding answers to questions like “How many coffees were sold today?” or “What was the cheapest drink sold this morning?” becomes slow and difficult.



The owner has to read through many pages and count orders manually. This is where computers and databases become useful.



What Is a Database ?



* Think of a database as a place where a computer stores information in an organised way.



* You can think of a database as a digital notebook that never runs out of pages. Unlike a paper notebook, a database allows the computer to search, count, and sort information very quickly.



* Even if the café has thousands of orders, a database can still answer questions in seconds.



* Inside a database, information is stored in tables.



Tables, Columns, and Rows :-

\--------------------------



1. A table resembles a spreadsheet, where information is organised neatly into rows and columns.



2\. Columns are the titles at the top of the table. They describe the type of information stored.



3\. Rows go across the table. Each row contains one complete set of information.



For the café example :-

\--------------------



1. Columns might be: order number, drink, price, and time

2\. Each row is one café order



This means :-

\----------



* One column stores one type of information, such as prices
* One row stores all the information about a single order
* If the café sells ten drinks in one day, the table will contain ten rows. If one more customer places an order, one more row is added to the table.
* If an order is removed, only that row disappears. The rest of the table stays the same.



Asking Questions With SQL :-

\--------------------------

SQL is a language used to ask questions of a database. Instead of reading the table row by row, SQL lets the computer do the work for us.



For example, the café owner might ask :-

\-------------------------------------



* “Show me all orders.”
* “Show me only coffee orders.”
* “Show me the cheapest drink.”



These questions are called queries. A query does not change the data. It only displays the requested information from the table.







Answer the questions below:

Inside databases, what is the term for the "spreadsheets" that store the information?



Answer : Table

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Writing Your First SQL Query :-

\-----------------------------

The Café SQL website will appear in split view on the right side of your browser. In case split view is not visible, press the Show Split View button at the top of the page.



At the top of the page, you can see the two tables and their columns:



* Orders (id,drink,price,time)
* Menu (drink, price)



Your goal is to practise writing queries using four core SQL parts: SELECT, FROM, WHERE, and ORDER BY.



Step 1: View Everything in a Table (Select + From):-

\--------------------------------------------------

We start with the most basic query. When we use SELECT \*, the \* symbol means all columns. The word FROM tells the database which table to use.



Try this query :-

\--------------

SELECT \* FROM Orders;



* Click Run Query. You should see every order currently stored in the database.
* Café SQL app running SELECT \* FROM Orders, returning 50 rows with id, drink, price, and time columns



Step 2: Show Only Specific Columns (Select Drink, Price) :-

\--------------------------------------------------------

Sometimes we do not need every column. We can choose specific columns by listing them after SELECT.



Try this query :-

\--------------

SELECT drink, price FROM Orders;



* This will display only the drink and price columns.
* Café SQL app running SELECT drink, price FROM Orders, returning 50 rows showing only the drink and price columns



Step 3: Filter Results (Where) :-

\-------------------------------

The WHERE keyword filters rows. It keeps only rows that match a condition.



Try filtering by drink name :-

\---------------------------

SELECT \* FROM Orders WHERE drink = 'Coffee';



* If the database contains coffee orders, you will now see only those rows.
* Café SQL app running SELECT \* FROM Orders WHERE drink = 'Coffee', returning 10 filtered rows of Coffee orders



Hint: If you are not sure which drink names exist, run:

\----

SELECT \* FROM Menu;



Step 4: Sort Results (Order By) :-

\--------------------------------

The ORDER BY keyword sorts results by a column. By default, results are sorted in ascending order (lowest to highest).



Try sorting orders by price (lowest first) :-

\------------------------------------------

SELECT \* FROM Orders ORDER BY price;



* Café SQL app running SELECT \* FROM Orders ORDER BY price, returning rows sorted by price from lowest to highest
* To sort in reverse order (highest to lowest), add DESC.



Try sorting orders by price (highest first) :-

\-------------------------------------------

SELECT \* FROM Orders ORDER BY price DESC;



* Café SQL app running SELECT \* FROM Orders ORDER BY price DESC, returning rows sorted by price from highest to lowest



Step 5: Combine Filtering + Sorting :-

\------------------------------------

Most real queries combine parts together. Here, we filter to keep only one drink type and then sort by price.



Try this query :-

\--------------

SELECT \* FROM Orders WHERE drink = 'Coffee' ORDER BY price DESC;



* Café SQL app running SELECT \* FROM Orders WHERE drink = 'Coffee' ORDER BY price DESC, returning 10 Coffee orders sorted by price descending



Answer the questions below:

When you showed all orders, how many rows were returned?



Answer : 50

\------



When you sorted orders by price from cheapest to most expensive, which drink appeared first?



Answer : Tea

\------



When you sorted the menu by price from most expensive to cheapest, which drink appeared first?



Answer : Latte

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conclusion :-

\----------

In this room, we learned how computers store information in databases and how SQL is used to ask clear questions about that information. Using a café example, we saw how tables organise orders into rows and columns, and how simple SQL commands can show, filter, sort, and add data.



Skills Learned :-

\--------------

* Understanding what a database is
* Knowing what tables, rows, and columns are
* Asking simple questions using SQL
* Reading results returned by a database
* SQL Queries Learned in This Room



1. SELECT – choose what data to display



2\. FROM – choose where the data comes from



3\. WHERE – filter records based on a condition



4\. ORDER BY – sort results



Question to think about :-

\-----------------------



1. What could happen if someone were allowed to change or remove café orders without permission?



Answer : Allowing unauthorized changes or deletions to café orders compromises data integrity and opens the door to serious operational and financial risks. Financial fraud is a major concern; someone could alter prices, delete paid orders, or pocket cash without leaving a trace. Operationally, it causes fulfillment chaos—if the kitchen loses track of active orders or inventory counts get skewed, customers receive the wrong items, ingredients run out unexpectedly, and waste skyrockets. From a business perspective, it destroys the audit trail, making it impossible to reconcile daily revenue, investigate losses, or hold anyone accountable. In cybersecurity terms, this is a textbook violation of the integrity pillar of the CIA triad, demonstrating precisely why strict access controls, user authentication, and permission management are vital for any database.



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

What is Networking? Room :-

\-------------------------

Task 1 :-

\------

What is Networking?



Answer : Networks are simply things connected. For example, your friendship circle: you are all connected because of similar interests, hobbies, skills and sorts.

\------



Networks can be found in all walks of life:



* A city's public transportation system
* Infrastructure such as the national power grid for electricity
* Meeting and greeting your neighbours
* Postal systems for sending letters and parcels



But more specifically, in computing, networking is the same idea, just dispersed to technological devices. Take your phone as an example; the reason that you have it is to access things. We'll cover how these devices communicate with each other and the rules that follow.



In computing, a network can be formed by anywhere from 2 devices to billions. These devices include everything from your laptop and phone to security cameras, traffic lights and even farming!



Networks are integrated into our everyday life. Be it gathering data for the weather, delivering electricity to homes or even determining who has the right of way at a road. Because networks are so embedded in the modern-day, networking is an essential concept to grasp in cybersecurity.



Answer the questions below:

What is the key term for devices that are connected together?



Answer : network

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

What is the Internet?



Answer : Now that we've learnt what a network is and how one is defined in computing (just devices connected), let's explore the Internet.

\-------



The Internet is one giant network that consists of many, many small networks within itself. Using our example from the previous task, let's now imagine that Alice made some new friends named Zayn and Toby that she wants to introduce to Bob and Jim. The problem is that Alice is the only person who speaks the same language as Zayn and Toby. So Alice will have to be the messenger!



Because Alice can speak both languages, they can communicate to one another through Alice — forming a new network.



The first iteration of the Internet was within the ARPANET project in the late 1960s. This project was funded by the United States Defence Department and was the first documented network in action. However, it wasn't until 1989 when the Internet as we know it was invented by Tim Berners-Lee by the creation of the World Wide Web (WWW). It wasn't until this point that the Internet started to be used as a repository for storing and sharing information, just like it is today.



As previously stated, the Internet is made up of many small networks all joined together.  These small networks are called private networks, where networks connecting these small networks are called public networks -- or the Internet! So, to recap, a network can be one of two types:



1. A private network

2\. A public network



Devices will use a set of labels to identify themselves on a network, which we will come onto in the task below.



Answer the questions below:

Who invented the World Wide Web?



Answer :  Tim Berners-Lee

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Identifying Devices on a Network :-

\---------------------------------

To communicate and maintain order, devices must be both identifying and identifiable on a network. What use is it if you don't know whom you're talking to at the end of the day?



Devices on a network are very similar to humans in the fact that we have two ways of being identified:



* Our Name
* Our Fingerprints



Now we can change our name through deed poll, but we can't, however, change our fingerprints. Every human has an individual set of fingerprints which means that even if they change their name, there is still an identity behind it. Devices have the same thing: two means of identification, with one being permeable. These are:



1. An IP Address

2\. A Media Access Control (MAC) Address -- think of this as being similar to a serial number.



IP Addresses :-

\------------

Briefly, an IP address (or Internet Protocol) address can be used as a way of identifying a host on a network for a period of time, where that IP address can then be associated with another device without the IP address changing. First, let's split up precisely what an IP address is in the diagram below:



An IP address is a set of numbers that are divided into four octets. The value of each octet will summarise to be the IP address of the device on the network. This number is calculated through a technique known as IP addressing \& subnetting, but that is for another day. What's important to understand here is that IP addresses can change from device to device but cannot be active simultaneously more than once within the same network.



IP Addresses follow a set of standards known as protocols. These protocols are the backbone of networking and force many devices to communicate in the same language, which is something that we'll come onto another time. However, we should recall that devices can be on both a private and public network. Depending on where they are will determine what type of IP address they have: a public or private IP address.



A public address is used to identify the device on the Internet, whereas a private address is used to identify a device amongst other devices. Take the table \& screenshot below as an example. Here we have two devices on a private network:



|Device Name|IP Address|IP Address Type|
|-|-|-|
|DESKTOP-KJE57FD|192.168.1.77|Private|
|DESKTOP-KJE57FD|86.157.52.21|Public|
|CMNatic-PC|192.168.1.74|Private|
|CMNatic-PC|86.157.52.21|Public|



These two devices will be able to use their private IP addresses to communicate with each other. However, any data sent to the Internet from either of these devices will be identified by the same public IP address. Public IP addresses are given by your Internet Service Provider (or ISP) at a monthly fee (your bill!)



As more and more devices become connected, it is becoming increasingly harder to get a public address that isn't already in use. For example, Cisco, an industry giant in the world of networking, estimated that there would be approximately 50 billion devices connected on the Internet by the end of 2021. (Cisco., 2021)(opens in new tab). Enter IP address versions. So far, we have only discussed one version of the Internet Protocol addressing scheme known as IPv4, which uses a numbering system of 2^32 IP addresses (4.29 billion) -- so you can see why there is such a shortage!



IPv6 is a new iteration of the Internet Protocol addressing scheme to help tackle this issue. Although it is seemingly more daunting, it boasts a few benefits:



* Supports up to 2^128 of IP addresses (340 trillion-plus), resolving the issues faced with IPv4
* More efficient due to new methodologies



MAC Addresses :-

\--------------

Devices on a network will all have a physical network interface, which is a microchip board found on the device's motherboard. This network interface is assigned a unique address at the factory it was built at, called a MAC (Media Access Control ) address. The MAC address is a twelve-character hexadecimal number (a base sixteen numbering system used in computing to represent numbers) split into two's and separated by a colon. These colons are considered separators. For example, a4:c3:f0:85:ac:2d. The first six characters represent the company that made the network interface, and the last six is a unique number.



However, an interesting thing with MAC addresses is that they can be faked or "spoofed" in a process known as spoofing. This spoofing occurs when a networked device pretends to identify as another using its MAC address. When this occurs, it can often break poorly implemented security designs that assume that devices talking on a network are trustworthy. Take the following scenario: A firewall is configured to allow any communication going to and from the MAC address of the administrator. If a device were to pretend or "spoof" this MAC address, the firewall would now think that it is receiving communication from the administrator when it isn't.



Places such as cafes, coffee shops, and hotels alike often use MAC address control when using their "Guest "or "Public" Wi-Fi. This configuration could offer better services, i.e. a faster connection for a price if you are willing to pay the fee per device.  The interactive lab attached to this task has been made to replicate this scenario!



Practical :-

\---------

The interactive labs simulate a hotel Wi-Fi network where you have to pay for the service. You'll note that the router is not allowing Bob's packets ( blue) to the TryHackMe website and is placing them in the bin, but Alice's packets (green) are going through fine because she has paid for Wi-Fi. Try changing Bob's MAC address to the same as Alice's to see what happens.



Lab :-

\---

Step-1 :-

\-------

we see the following scenario where r1 connected to a switch and that switch connected to bob and alice and The interactive labs simulate a hotel Wi-Fi network where you have to pay for the service. You'll note that the router is not allowing Bob's packets ( blue) to the TryHackMe website and is placing them in the bin, but Alice's packets (green) are going through fine because she has paid for Wi-Fi.



BOB Mac Address --- 04:9E:44:99:A3:12

ALICE Mac Address --- 00:12:32:2F:33:39

&#x20;

Step-2 :-

\------

Now we copy alice Mac address and set in bob machine

BOB Mac Address --- 00:12:32:2F:33:39

ALICE Mac Address --- 00:12:32:2F:33:39



Step-3 :-

\------

Now when BOB send request then the blue bob packets reach router instead of drop them in bin and after the we get the flag THM{YOU\_GOT\_ON\_TRYHACKME} and our final 4th number question is solve.



Note :-

\-----

ip is unique so one ip can be used in one device not in another but one MAC can be copied and placed into another device like how we do in real world our machine mac we set in our home router and then our router get internet. Here BOB MAC address is blocked so router drop the packet but alice MAC address not allowed so when use alice MAC address in BOB then teh packet router not discard and send in bin.



Answer the questions below:

What does the term "IP" stand for?



Answer : Internet Protocol

\------



What is each section of an IP address called?



Answer : Octet

\------



How many sections (in digits) does an IPv4 address have?



Answer : 4

\------



What does the term "MAC" stand for?



Answer : Media Access Control

\------



Deploy the interactive lab using the "View Site" button and spoof your MAC address to access the site.  What is the flag?



Answer : THM{YOU\_GOT\_ON\_TRYHACKME}

\------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Ping (ICMP) :-

\-----------

* Ping is one of the most fundamental network tools available to us. Ping uses ICMP (Internet Control Message Protocol) packets to determine the performance of a connection between devices, for example, if the connection exists or is reliable.



* The time taken for ICMP packets travelling between devices is measured by ping, such as in the screenshot below. This measuring is done using ICMP's echo packet and then ICMP's echo reply from the target device.



* Pings can be performed against devices on a network, such as your home network or resources like websites. This tool can be easily used and comes installed on Operating Systems (OSs) such as Linux and Windows. The syntax to do a simple ping is ping IP address or website URL.



* Suppose we are pinging a device that has the private address of 192.168.1.254. Ping informs us that we have sent six ICMP packets, all of which were received with an average time of 4.16 milliseconds.



Now you are going to do the same thing to ping the address of "8.8.8.8" on the deployable website in this task. Pinging the correct address will reveal a flag to answer the following question below.



Lab :-

\----

here we give command ping-c 4 (for send 4 packets) 8.8.8.8 and after ping successful under it we get the flag Flag: THM{I\_PINGED\_THE\_SERVER} that is our forth question answer.

\----------------------------------------------------------------

user@thm:\~$ ping -c 4 8.8.8.8

PING 8.8.8.8 (8.8.8.8) 56(84) bytes of data

64 bytes from 8.8.8.8: icmp\_seq=1 ttl=56 time=7.84 ms

64 bytes from 8.8.8.8: icmp\_seq=1 ttl=56 time=7.18 ms

64 bytes from 8.8.8.8: icmp\_seq=1 ttl=56 time=8.40 ms

64 bytes from 8.8.8.8: icmp\_seq=1 ttl=56 time=7.68 ms

\--- 8.8.8.8 ping statistics ---

4 packets transmitted, 4 received, 0% packet loss, time 4006ms

rtt min/avg/max/mdev = 8.132/9.428/10.957/1.057 ms

Flag: THM{I\_PINGED\_THE\_SERVER}

\----------------------------------------------------------------



Answer the questions below:

What protocol does ping use?

&#x20;

Answer : ICMP

\------



What is the syntax to ping 10.10.10.10?



Answer : ping 10.10.10.10

\------



What flag do you get when you ping 8.8.8.8?



Answer : THM{I\_PINGED\_THE\_SERVER}

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Intro to LAN Room :-

\-----------------

Task 1 :-

\-------

Introducing LAN Topologies :-

\---------------------------

Local Area Network (LAN) Topologies :-

\------------------------------------

Over the years, there has been experimentation and implementation of various network designs. In reference to networking, when we refer to the term "topology", we are actually referring to the design or look of the network at hand. Let's discuss the advantages and disadvantages of these topologies below.



Star Topology :-

\--------------

The main premise of a star topology is that devices are individually connected via a central networking device such as a switch or hub. This topology is the most commonly found today because of its reliability and scalability - despite the cost.



Any information sent to a device in this topology is sent via the central device to which it connects. Let's explore some of these advantages and disadvantages of this topology below:



Because more cabling and the purchase of dedicated networking equipment is required for this topology, it is more expensive than any of the other topologies. However, despite the added cost, this does provide some significant advantages. For example, this topology is much more scalable in nature, which means that it is very easy to add more devices as the demand for the network increases.



Unfortunately, the more the network scales, the more maintenance is required to keep the network functional. This increased dependence on maintenance can also make troubleshooting faults much harder. Furthermore, the star topology is still prone to failure - albeit reduced. For example, if the centralised hardware that connects devices fails, these devices will no longer be able to send or receive data. Thankfully, these centralised hardware devices are often robust.



Bus Topology :-

\-------------

This type of connection relies upon a single connection which is known as a backbone cable. This type of topology is similar to the leaf off of a tree in the sense that devices (leaves) stem from where the branches are on this cable.



Because all data destined for each device travels along the same cable, it is very quickly prone to becoming slow and bottlenecked if devices within the topology are simultaneously requesting data. This bottleneck also results in very difficult troubleshooting because it quickly becomes difficult to identify which device is experiencing issues with data all travelling along the same route.



However, with this said, bus topologies are one of the easier and more cost-efficient topologies to set up because of their expenses, such as cabling or dedicated networking equipment used to connect these devices.



Lastly, another disadvantage of the bus topology is that there is little redundancy in place in case of failures. This disadvantage is because there is a single point of failure along the backbone cable. If this cable were to break, devices can no longer receive or transmit data along the bus.



Ring Topology :-

\--------------

The ring topology (also known as token topology) boasts some similarities. Devices such as computers are connected directly to each other to form a loop, meaning that there is little cabling required and less dependence on dedicated hardware such as within a star topology.



A ring topology works by sending data across the loop until it reaches the destined device, using other devices along the loop to forward the data. Interestingly, a device will only send received data from another device in this topology if it does not have any to send itself. If the device happens to have data to send, it will send its own data first before sending data from another device.



Because there is only one direction for data to travel across this topology, it is fairly easy to troubleshoot any faults that arise. However, this is a double-edged sword because it isn't an efficient way of data travelling across a network, as it may have to visit many multiple devices first before reaching the intended device.



Lastly, ring topologies are less prone to bottlenecks, such as within a bus topology, as large amounts of traffic are not travelling across the network at any one time. The design of this topology does, however, mean that a fault such as cut cable, or broken device will result in the entire networking breaking.



1. What is a Switch?

Answer : Switches are dedicated devices within a network that are designed to aggregate multiple other devices such as computers, printers, or any other networking-capable device using ethernet. These various devices plug into a switch's port. Switches are usually found in larger networks such as businesses, schools, or similar-sized networks, where there are many devices to connect to the network. Switches can connect a large number of devices by having ports of 4, 8, 16, 24, 32, and 64 for devices to plug into.



Switches are much more efficient than their lesser counterpart (hubs/repeaters). Switches keep track of what device is connected to which port. This way, when they receive a packet, instead of repeating that packet to every port like a hub would do, it just sends it to the intended target, thus reducing network traffic.







Both Switches and Routers can be connected to one another. The ability to do this increases the redundancy (the reliability) of a network by adding multiple paths for data to take. If one path goes down, another can be used. Whilst this may reduce the overall performance of a network because packets have to take longer to travel, there is no downtime -- a small price to pay considering the alternative.



2\. What is a Router?

Answer : It's a router's job to connect networks and pass data between them. It does this by using routing (hence the name router!).



Routing is the label given to the process of data travelling across networks. Routing involves creating a path between networks so that this data can be successfully delivered.



Routing is useful when devices are connected by many paths, such as in the example diagram below.



Lab :-

\----

what are the topology disadvantages :-

\------------------------------------

1. Ring topology :-

&#x20;  --------------

In a ring topology, all devices are a connector to two others to create a full circle. Packets of data travel from one device to the next until they have reached their destination. One of the major flaws with a ring topology is that if a device goes down or a cable is broken, then data will no longer be passed. If you hover over the middle of the network cable, you can cut it then The packets can now no longer travel around the network, and no devices can talk to each other.



2\. Bus Topology :-

&#x20;  -------------

With a bus topology, all devices are connected to a single cable, often called the backbone. Data is sent in both left and right directions down the backbone until the packet's destination is reached. A major flaw in the bus topology is that it can't handle a large amount of data. On the next step, send as many packets as quickly as you can to try and take down the network. so after send many packets that topology going to down.



3\. Star Topology :-

&#x20;  --------------

With a star topology, all devices are connected with their own cable to a central switch/hub. Every packet is sent through this switch, which means if the switch goes down the network will no longer work. Now here if switch any how destroy or not work then this topology gonna down.



Answer the questions below:

What does LAN stand for?



Answer : Local Area Network

\-------



What is the verb given to the job that Routers perform?



Answer : Routing

\-------



What device is used to centrally connect multiple devices on the local network and transmit data to the correct location?



Answer : Switch

\-------



What topology is cost-efficient to set up?



Answer : Bus Topology

\-------



What topology is expensive to set up and maintain?



Answer : Star Topology

\-------



Complete the interactive lab attached to this task. What is the flag given at the end?



Answer :

\-------

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

A Primer on Subnetting :-

\----------------------

As we've previously discussed throughout the module so far, Networks can be found in all shapes and sizes - ranging from small to large. Subnetting is the term given to splitting up a network into smaller, miniature networks within itself. Think of it as slicing up a cake for your friends. There's only a certain amount of cake to go around, but everybody wants a piece. Subnetting is you deciding who gets what slice \& reserving such a slice of this metaphorical cake.



Take a business, for example; You will have different departments such as:



* Accounting
* Finance
* Human Resources





Whilst you know where to send information in real life to the correct department, networks need to know as well. Network administrators use subnetting to categorise and assign specific parts of a network to reflect this.



Subnetting is achieved by splitting up the number of hosts that can fit within the network, represented by a number called a subnet mask. Let's refer back to our diagram from the first room in this module:



As we can recall, an IP address is made up of four sections called octets. The same goes for a subnet mask which is also represented as a number of four bytes (32 bits), ranging from 0 to 255 (0-255).



Subnets use IP addresses in three different ways:



* Identify the network address
* Identify the host address
* Identify the default gateway



Let's split these three up to understand their purposes into the table below:



|Type|Purpose|Explanation|Example|
|-|-|-|-|
|Network Address|This address identifies the start of the actual network and is used to identify a network's existence.|For example, a device with the IP address of 192.168.1.100 will be on the network identified by 192.168.1.0|192.168.1.0|
|Host Address|An IP address here is used to identify a device on the subnet|For example, a device will have the network address of 192.168.1.1|192.168.1.100|
|Default Gateway|The default gateway address is a special address assigned to a device on the network that is capable of sending information to another network|Any data that needs to go to a device that isn't on the same network (i.e. isn't on 192.168.1.0) will be sent to this device. These devices can use any host address but usually use either the first or last host address in a network (.1 or .254)|192.168.1.254<br />|



Now, in small networks such as at home, you will be on one subnet as there is an unlikely chance that you need more than 254 devices connected at one time.



However, places such as businesses and offices will have much more of these devices (PCs, printers, cameras and sensors), where subnetting takes place.



Subnetting provides a range of benefits, including:



* Efficiency
* Security
* Full control



We'll come on to explore exactly how subnetting provides these benefits at a later date; however, for now, all we need to understand is the security element to it. Let's take the typical café on the street. This cafe will have two networks:



* One for employees, cash registers, and other devices for the facility
* One for the general public to use as a hotspot



Subnetting allows you to separate these two use cases from each other whilst having the benefits of a connection to larger networks such as the Internet.



Answer the questions below:

1. What is the technical term for dividing a network up into smaller pieces?



Answer : Subnetting

\------



2\. How many bits are in a subnet mask?



Answer : 32

\------



3\. What is the range of a section (octet) of a subnet mask?



Answer : 0-255

\------



4\. What address is used to identify the start of a network?



Answer : Network Address

\------



5\. What address is used to identify devices within a network?



Answer : Host Address

\------



6\. What is the name used to identify the device responsible for sending data to another network?



Answer : Default Gateway

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

ARP (Address resolution protocol)  :-

\----------------------------------

Recalling from our previous tasks that devices can have two identifiers: A MAC address and an IP address, the Address Resolution Protocol or ARP for short, is the technology that is responsible for allowing devices to identify themselves on a network.



Simply, ARP allows a device to associate its MAC address with an IP address on the network. Each device on a network will keep a log of the MAC addresses associated with other devices.



When devices wish to communicate with another, they will send a broadcast to the entire network searching for the specific device. Devices can use ARP to find the MAC address (and therefore the physical identifier) of a device for communication.



How does ARP Work?



Each device within a network has a ledger to store information on, which is called a cache. In the context of ARP, this cache stores the identifiers of other devices on the network.



In order to map these two identifiers together (IP address and MAC address), ARP sends two types of messages:



* ARP Request
* ARP Reply



When an ARP request is sent, a message is broadcasted on the network to other devices asking, "What is the mac address that owns this IP address?" When the other devices receive that message, they will only respond if they own that IP address and will send an ARP reply with its MAC address. The requesting device can now remember this mapping and store it in its ARP cache for future use.



Answer the questions below:

What does ARP stand for?



Answer : Address Resolution Protocol

\------

What category of ARP Packet asks a device whether or not it has a specific IP address?



Answer : Request

\------

What address is used as a physical identifier for a device on a network?



Answer : MAC Address

\------

What address is used as a logical identifier for a device on a network?



Answer : IP Address

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

DHCP :-

\-----

IP addresses can be assigned either manually, by entering them physically into a device, or automatically and most commonly by using a DHCP (Dynamic Host Configuration Protocol) server. When a device connects to a network, if it has not already been manually assigned an IP address, it sends out a request (DHCP Discover) to see if any DHCP servers are on the network. The DHCP server then replies back with an IP address the device could use (DHCP Offer). The device then sends a reply confirming it wants the offered IP Address (DHCP Request), and then lastly, the DHCP server sends a reply acknowledging this has been completed, and the device can start using the IP Address (DHCP ACK).



Answer the questions below :

What type of DHCP packet is used by a device to retrieve an IP address?



Answer : DHCP Discover

\------



What type of DHCP packet does a device send once it has been offered an IP address by the DHCP server?



Answer : DHCP Request

\-------



Finally, what is the last DHCP packet that is sent to a device from a DHCP server?



Answer : DHCP ACK

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

OSI Model Room :-

\---------------

Task 1 :-

\------

1. What is the OSI Model?



Answer : The OSI model (or Open Systems Interconnection Model) is an essential model used in networking.  This critical model provides a framework dictating how all networked devices will send, receive and interpret data.



One of the main benefits of the OSI model is that devices can have different functions and designs on a network while communicating with other devices. Data sent across a network that follows the uniformity of the OSI model can be understood by other devices.



The OSI model consists of seven layers which are illustrated in the diagram below. Each layer has a different set of responsibilities and is arranged from Layer 7 to Layer 1.



At every individual layer that data travels through, specific processes take place, and pieces of information are added to this data, which is what we'll come to discuss in the upcoming tasks within this room. However, for now, we only need to understand that this process is called encapsulation and what the OSI model looks like in the diagram below:



Answer the questions below:

1. What does the "OSI" in "OSI Model" stand for?



Answer : Open Systems Interconnection



\-------

2\. How many layers (in digits) does the OSI model have?



Answer : 7

\-------



3\. What is the key term for when pieces of information get added to data?



Answer : encapsulation

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Layer 1 - Physical :-

\-------------------

This layer is one of the easiest layers to grasp. Put simply, this layer references the physical components of the hardware used in networking and is the lowest layer that you will find. Devices use electrical signals to transfer data between each other in a binary numbering system (1's and 0's).



For example, ethernet cables connecting devices.



Answer the questions below:

What is the name of this Layer?



Answer : Physical

\-------



What is the name of the numbering system that is both 0's and 1's?



Answer : Binary

\-------



What is the name of the cables that are used to connect devices?



Answer : Ethernet Cables

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Layer 2 - Data Link :-

\--------------------

The data link layer focuses on the physical addressing of the transmission. It receives a packet from the network layer (including the IP address for the remote computer) and adds in the physical MAC (Media Access Control) address of the receiving endpoint. Inside every network-enabled computer is a Network Interface Card (NIC) which comes with a unique MAC address to identify it.



MAC addresses are set by the manufacturer and literally burnt into the card; they can’t be changed – although they can be spoofed. When information is sent across a network, it’s actually the physical address that is used to identify where exactly to send the information.



Additionally, it’s also the job of the data link layer to present the data in a format suitable for transmission.



Answer the questions below:

What is the name of this Layer?



Answer : Data Link

\------



What is the name of the piece of hardware that all networked devices come with?



Answer : Network Interface Card

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Layer 3 - Network :-

\-----------------

The third layer of the OSI model (network layer) is where the magic of routing \& re-assembly of data takes place (from these small chunks to the larger chunk). Firstly, routing simply determines the most optimal path in which these chunks of data should be sent.



Whilst some protocols at this layer determine exactly what is the "optimal" path that data should take to reach a device, we should only know about their existence at this stage of the networking module. Briefly, these protocols include OSPF (Open Shortest Path First) and RIP (Routing Information Protocol). The factors that decide what route is taken is decided by the following:



* What path is the shortest? I.e. has the least amount of devices that the packet needs to travel across.
* What path is the most reliable? I.e. have packets been lost on that path before?
* Which path has the faster physical connection? I.e. is one path using a copper connection (slower) or a fibre (considerably faster)?



At this layer, everything is dealt with via IP addresses such as 192.168.1.100. Devices such as routers capable of delivering packets using IP addresses are known as Layer 3 devices — because they are capable of working at the third layer of the OSI model.



Answer the questions below:

1. What is the name of this Layer?



Answer : Network

\-------



2\. Will packets take the most optimal route across a network? (Y/N)



Answer : Y

\-------



3\. What does the acronym "OSPF" stand for?



Answer : Open Shortest Path First

\-------



4\. What does the acronym "RIP" stand for?



Answer : Routing Information Protocol

\-------



5\. What type of addresses are dealt with at this layer?



Answer : IP Addresses

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\-------

Layer 4 - Transport :-

\-------------------

Layer 4 of the OSI model plays a vital part in transmitting data across a network and can be a little bit difficult to grasp. When data is sent between devices, it follows one of two different protocols that are decided based upon several factors:



* TCP
* UDP



Let's begin with TCP. The Transmission Control Protocol (TCP). Potentially hinted by the name, this protocol is designed with reliability and guarantee in mind. This protocol reserves a constant connection between the two devices for the amount of time it takes for the data to be sent and received.



Not only this, but TCP incorporates error checking into its design. Error checking is how TCP can guarantee that data sent from the small chunks in the session layer (layer 5) has then been received and reassembled in the same order.



Let's summarise the advantages and disadvantages of TCP in the table below:



|Advantages of TCP|<br />Disadvantages of TCP|
|-|-|
|Guarantees the accuracy of data.|Requires a reliable connection between the two devices. If one small chunk of data is not received, then the entire chunk of data cannot be used.|
|Capable of synchronising two devices to prevent each other from being flooded with data.|A slow connection can bottleneck another device as the connection will be reserved on the receiving computer the whole time.|
|Performs a lot more processes for reliability.|<br />TCP is significantly slower than UDP because more work has to be done by the devices using this protocol.|



TCP is used for situations such as file sharing, internet browsing or sending an email. This usage is because these services require the data to be accurate and complete (no good having half a file!).



Now let's move onto the User Datagram Protocol (or UDP for short). This protocol is not nearly as advanced as its brother - the TCP protocol. It doesn't boast the many features offered by TCP, such as error checking and reliability. In fact, any data that gets sent via UDP is sent to the computer whether it gets there or not. There is no synchronisation between the two devices or guarantee; just hope for the best, and fingers crossed.



Whilst this sounds disadvantageous, it does have its merits, which we'll layout in the table below:



|Advantages of UDP|Disadvantages of UDP|
|-|-|
|UDP is much faster than TCP.|UDP doesn't care if the data is received.|
|UDP leaves the application layer (user software) to decide if there is any control over how quickly packets are sent.|It is quite flexible to software developers in this sense.|
|UDP does not reserve a continuous connection on a device as TCP does.|This means that unstable connections result in a terrible experience for the user.|



UDP is useful in situations where there are small pieces of data being sent. For example, protocols used for discovering devices (ARP and DHCP that we discussed in Room 2 - Intro to LAN) or larger files such as video streaming (where it is okay if some part of the video is pixelated. Pixels are just lost pieces of data!)



Answer the questions below:

1. What is the name of this Layer?



Answer : Transport

\------



2\. What does TCP stand for?



Answer : Transmission Control Protocol

\------



3\. What does UDP stand for?



Answer : User Datagram Protocol

\------



4\. What protocol guarantees the accuracy of data?



Answer : TCP

\------



5\. What protocol doesn't care if data is received or not by the other device?



Answer : UDP

\------



6\. What protocol would an application such as an email client use?



Answer : TCP

\------



7\. What protocol would an application that downloads files use?



Answer : TCP

\------



8\. What protocol would an application that streams video use?



Answer : UDP

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 6 :-

\-------

Layer 5 - Session :-

\-----------------

Once data has been correctly translated or formatted from the presentation layer (layer 6), the session layer (layer 5) will begin to create and maintain the connection to other computer for which the data is destined. When a connection is established, a session is created. Whilst this connection is active, so is the session.



The session layer is also responsible for closing the connection if it hasn't been used in a while or if it is lost. Additionally, a session can contain "checkpoints," where if the data is lost, only the newest pieces of data are required to be sent, saving bandwidth.



What is worthy of noting is that sessions are unique — meaning that data cannot travel over different sessions, but in fact, only across each session instead.



Answer the questions below:

What is the name of this layer?



Answer : Session

\-------



What is the technical term for when a connection is succesfully established?



Answer : Session

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 7 :-

\-------

Layer 6 - Presentation :-

\-----------------------

Layer 6 of the OSI model is the layer in which standardisation starts to take place. Because software developers can develop any software such as an email client differently, the data still needs to be handled in the same way — no matter how the software works.



This layer acts as a translator for data to and from the application layer (layer 7). The receiving computer will also understand data sent to a computer in one format destined for in another format. For example, when you send an email, the other user may have another email client to you, but the contents of the email will still need to display the same.



Security features such as data encryption (like HTTPS when visiting a secure site) occur at this layer.



Answer the questions below:

What is the name of this Layer?



Answer : Presentation

\-------



What is the main purpose that this Layer acts as?



Answer : Translator

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 8 :-

\-------

Layer 7 - Application :-

\----------------------

The application layer of the OSI model is the layer that you will be most familiar with. This familiarity is because the application layer is the layer in which protocols and rules are in place to determine how the user should interact with data sent or received.



Everyday applications such as email clients, browsers, or file server browsing software such as FileZilla provide a friendly, Graphical User Interface (GUI) for users to interact with data sent or received. Other protocols include DNS (Domain Name System), which is how website addresses are translated into IP addresses.



Answer the questions below:

What is the name of this Layer?



Answer : Application

\------



What is the technical term that is given to the name of the software that users interact with?



Answer : Graphical User Interface

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Packets \& Frames Room :-

\----------------------

Task 1 :-

\-------

What are Packets and Frames :-

\----------------------------

Packets and frames are small pieces of data that, when forming together, make a larger piece of information or message. However, they are two different things in the OSI model.



A packet is a piece of data from Layer 3 (Network Layer) of the OSI model, containing information such as an IP header and payload. A frame, however, is used at Layer 2 (Data Link) of the OSI model, which, encapsulates the packet and adds additional information such as MAC addresses.



You can think of this process as similar to mailing a letter through the post. The envelope is a frame, which, is used to move the contents (in this analogy, the packet) of the envelope to another place. Once the recepient opens the envelop (frame), they will know how to forward the letter (packet) itself.



This process is called encapsulation which we discussed in room 3: the OSI model. At this stage, it's safe to assume that when we are talking about anything IP addresses, we are talking about packets. When the encapsulating information is stripped away, we're talking about the frame itself.



Packets are an efficient way of communicating data across networked devices such as those explained in Task 1. Because this data is exchanged in small pieces, there is less chance of bottlenecking occurring across a network than large messages being sent at once.



For example, when loading an image from a website, this image is not sent to your computer as a whole, but rather small pieces where it is reconstructed on your computer. Take the image below as an illustration of this process. The cat's picture is divided into three packets, where it is reconstructed when it reaches the computer to form the final image.



Packets have different structures that are dependant upon the type of packet that is being sent. As we'll come on to discuss, networking is full of standards and protocols that act as a set of rules for how the packet is handled on a device. With billions of devices connected on the internet, things can quickly break down if there is no standardisation.



Let's continue with our example of the Internet Protocol. A packet using this protocol will have a set of headers that contain additional pieces of information to the data that is being sent across a network.



Some notable headers include:



|Header|Description|
|-|-|
|Time to Live|This field sets an expiry timer for the packet to not clog up your network if it never manages to reach a host or escape!|
|Checksum|This field provides integrity checking for protocols such as TCP/IP. If any data is changed, this value will be different from what was expected and therefore corrupt.|
|Source Address|The IP address of the device that the packet is being sent from so that data knows where to return to.|
|Destination Address|The device's IP address the packet is being sent to so that data knows where to travel next.|



Answer the questions below:

What is the name for a piece of data when it does have IP addressing information?



Answer : Packet

\-------



What is the name for a piece of data when it does not have IP addressing information?



Answer : Frame

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

TCP/IP (The Three-Way Handshake) :-

\--------------------------------

TCP (or Transmission Control Protocol for short) is another one of these rules used in networking.



This protocol is very similar to the OSI model that we have previously discussed in room three of this module so far. The TCP/IP protocol consists of four layers and is arguably just a summarised version of the OSI model. These layers are:



* Application
* Transport
* Internet



Network Interface :-

\------------------

Very similar to how the OSI model works, information is added to each layer of the TCP model as the piece of data (or packet) traverses it. As you may recall, this process is known as encapsulation - where the reverse of this process is decapsulation.



One defining feature of TCP is that it is connection-based, which means that TCP must establish a connection between both a client and a device acting as a server before data is sent.



Because of this, TCP guarantees that any data sent will be received on the other end. This process is named the Three-way handshake, which is something we'll come on to discuss shortly. A table comparing the advantages and disadvantages of TCP is located below:



|Advantages of TCP|Disadvantages of TCP|
|-|-|
|Guarantees the integrity of data.|Requires a reliable connection between the two devices. If one small chunk of data is not received, then the entire chunk of data cannot be used and must be re-sent.|
|Capable of synchronising two devices to prevent each other from being flooded with data in the wrong order.|A slow connection can bottleneck another device as the connection will be reserved on the other device the whole time.|
|Performs a lot more processes for reliability|TCP is significantly slower than UDP because more work (computing) has to be done by the devices using this protocol.|



TCP packets contain various sections of information known as headers that are added from encapsulation. Let's explain some of the crucial headers in the table below:



|Header|Description|
|-|-|
|Source Port|This value is the port opened by the sender to send the TCP packet from. This value is chosen randomly (out of the ports from 0-65535 that aren't already in use at the time).|
|Destination Port|This value is the port number that an application or service is running on the remote host (the one receiving data); for example, a webserver running on port 80. Unlike the source port, this value is not chosen at random.|
|Source IP|This is the IP address of the device that is sending the packet.|
|Destination IP|This is the IP address of the device that the packet is destined for.|
|Sequence Number|When a connection occurs, the first piece of data transmitted is given a random number. We'll explain this more in-depth further on.|
|Acknowledgement Number|After a piece of data has been given a sequence number, the number for the next piece of data will have the sequence number + 1. We'll also explain this more in-depth further on.|
|Checksum|This value is what gives TCP integrity. A mathematical calculation is made where the output is remembered. When the receiving device performs the mathematical calculation, the data must be corrupt if the output is different from what was sent.|
|Data|This header is where the data, i.e. bytes of a file that is being transmitted, is stored.|
|Flag|This header determines how the packet should be handled by either device during the handshake process. Specific flags will determine specific behaviours, which is what we'll come on to explain below.|



Next, we'll come on to discuss the Three-way handshake - the term given for the process used to establish a connection between two devices. The Three-way handshake communicates using a few special messages - the table below highlights the main ones:



|Step|Message|Description|
|-|-|-|
|1|SYN|A SYN message is the initial packet sent by a client during the handshake. This packet is used to initiate a connection and synchronise the two devices together (we'll explain this further later on).|
|2|SYN/ACK|This packet is sent by the receiving device (server) to acknowledge the synchronisation attempt from the client.|
|3|ACK|The acknowledgement packet can be used by either the client or server to acknowledge that a series of messages/packets have been successfully received.|
|4|DATA|Once a connection has been established, data (such as bytes of a file) is sent via the "DATA" message.|
|5|FIN|This packet is used to cleanly (properly) close the connection after it has been complete.|
|6|RST|This packet abruptly ends all communication. This is the last resort and indicates there was some problem during the process. For example, if the service or application is not working correctly, or the system has faults such as low resources.|



Any sent data is given a random number sequence and is reconstructed using this number sequence and incrementing by 1. Both computers must agree on the same number sequence for data to be sent in the correct order. This order is agreed upon during three steps:



* SYN - Client :-

&#x20;  -------------

Here's my Initial Sequence Number(ISN) to SYNchronise with (0)



* SYN/ACK - Server :-

&#x20;  -----------------

Here's my Initial Sequence Number (ISN) to SYNchronise with (5,000), and I ACKnowledge your initial number sequence (0)



* ACK - Client :-

&#x20;  -------------

I ACKnowledge your Initial Sequence Number (ISN) of (5,000), here is some data that is my ISN+1 (0 + 1)



|Device|Initial Number Sequence (ISN)|Final Number Sequence|
|-|-|-|
|Client (Sender)|0|0 + 1 = 1|
|Client (Sender)|1|1 + 1 = 2|
|Client (Sender)|2|2 + 1 = 3|



TCP Closing a Connection :-

\-------------------------

Let's quickly explain the process behind TCP closing a connection. First, TCP will close a connection once a device has determined that the other device has successfully received all of the data.



Because TCP reserves system resources on a device, it is best practice to close TCP connections as soon as possible.



To initiate the closure of a TCP connection, the device will send a "FIN" packet to the other device. Of course, with TCP, the other device will also have to acknowledge this packet.



Answer the questions below:

1. What is the header in a TCP packet that ensures the integrity of data?



Answer :checksum

\-------



2\. Provide the order of a normal Three-way handshake (with each step separated by a comma)



Answer :SYN,SYN/ACK,ACK

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Practical - Handshake :-

\---------------------

Help Alice and Bob communicate by re-assembling the TCP handshake in the correct order.



Lab :-

\----

Step-1 :-

\-------

First Alice send SYN : Can you hear me Bob?

Step-2 :-

\-------

Now BoB send SYN/ACK : Yes, I can hear you!

Step-3 :-

\-------

Now Alice send ACK : Okay Great

Step-4 :-

\-------

Now Alice again send DATA : Cheesecake is on sale!

Step-5 :-

\-------

Now BOB send ACK : I Hear ya!

Step-6 :-

\-------

Now Alice send FIN/ACK : I'm all done

Step-7 :-

\-------

Now BOB send FIN/ACK : Yeah Me Too

Step-8 :-

\------

Now Alice send ACK : Okay, Goodbye

Step-9 :-

\-------



Answer the questions below :

What is the value of the flag given at the end of the conversation?



Answer : THM{TCP\_CHATTER}

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

UDP/IP :-

\-------

The User Datagram Protocol (UDP) is another protocol that is used to communicate data between devices. Unlike its brother TCP, UDP is a stateless protocol that doesn't require a constant connection between the two devices for data to be sent. For example, the Three-way handshake does not occur, nor is there any synchronisation between the two devices.



Recall some of the comparisons made about these two protocols in Room 3: "OSI Model". Namely, UDP is used in situations where applications can tolerate data being lost (such as video streaming or voice chat) or in scenarios where an unstable connection is not the end-all. A table comparing the advantages and disadvantages of UDP is located below:



|Advantages of UDP|Disadvantages of UDP|
|-|-|
|UDP is much faster than TCP.|UDP doesn't care if the data is received or not.|
|UDP leaves the application (user software) to decide if there is any control over how quickly packets are sent.|It is quite flexible to software developers in this sense.|
|UDP does not reserve a continuous connection on a device as TCP does.|This means that unstable connections result in a terrible experience for the user.|



As mentioned, no process takes place in setting up a connection between two devices. Meaning that there is no regard for whether or not data is received, and there are no safeguards such as those offered by TCP, such as data integrity.



UDP packets are much simpler than TCP packets and have fewer headers. However, both protocols share some standard headers, which are what is annotated in the table below:



|Header|Description|
|-|-|
|Time to Live (TTL)|This field sets an expiry timer for the packet, so it doesn't clog up your network if it never manages to reach a host or escape!|
|Source Address|The IP address of the device that the packet is being sent from, so that data knows where to return to.|
|Destination Address|The device's IP address the packet is being sent to so that data knows where to travel next.|
|Source Port|This value is the port that is opened by the sender to send the UDP packet from. This value is randomly chosen (out of the ports from 0-65535 that aren't already in use at the time).|
|Destination Port|This value is the port number that an application or service is running on the remote host (the one receiving the data); for example, a webserver running on port 80. Unlike the source port, this value is not chosen at random.|
|Data|This header is where data, i.e. bytes of a file that is being transmitted, is stored.|



Next, we'll come on to discuss how the process of a connection via UDP differs from that of something such as TCP.  We should recall that UDP is stateless. No acknowledgement is sent during a connection.



Answer the questions below:

1. What does the term "UDP" stand for?



Answer : User Datagram Protocol

\------



2\. What type of connection is "UDP"?



Answer : stateless

\------



3\. What protocol would you use to transfer a file?



Answer : TCP

\------



4\. What protocol would you use to have a video call?



Answer : UDP

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\-------

Ports 101 (Practical) :-

\---------------------

These ports enforce what can park and where — if it isn't compatible, it cannot park here. Networking devices also use ports to enforce strict rules when communicating with one another. When a connection has been established (recalling from the OSI model's room), any data sent or received by a device will be sent through these ports. In computing, ports are a numerical value between 0 and 65535 (65,535).



Because ports can range from anywhere between 0-65535, there quickly runs the risk of losing track of what application is using what port. A busy harbour is chaos! Thankfully, we associate applications, software and behaviours with a standard set of rules. For example, by enforcing that any web browser data is sent over port 80, software developers can design a web browser such as Google Chrome or Firefox to interpret the data the same way as one another.



This means that all web browsers now share one common rule: data is sent over port 80. How the browsers look, feel and easy to use is up to the designer or the user's decision.



While the standard rule for web data is port 80, a few other protocols have been allocated a standard rule. Any port that is within 0 and 1024 (1,024) is known as a common port. Let's explore some of these other protocols below:



|Protocol|Port Number|Description|
|-|-|-|
|File Transfer Protocol (FTP)|21|This protocol is used by a file-sharing application built on a client-server model, meaning you can download files from a central location.|
|Secure Shell (SSH)|22|This protocol is used to securely login to systems via a text-based interface for management.|
|HyperText Transfer Protocol (HTTP)|80|This protocol powers the World Wide Web (WWW)! Your browser uses this to download text, images and videos of web pages.|
|HyperText Transfer Protocol Secure (HTTPS)|443|This protocol does the exact same as above; however, securely using encryption.|
|Server Message Block (SMB)|445|This protocol is similar to the File Transfer Protocol (FTP); however, as well as files, SMB allows you to share devices like printers.|
|Remote Desktop Protocol (RDP)|3389|This protocol is a secure means of logging in to a system using a visual desktop interface (as opposed to the text-based limitations of the SSH protocol).|



What is worth noting here is that these protocols only follow the standards. I.e. you can administer applications that interact with these protocols on a different port other than what is the standard (running a web server on 8080 instead of the 80 standard port). Note, however, applications will presume that the standard is being followed, so you will have to provide a colon (:) along with the port number.



Practical Challenge :-

\-------------------

Open the site attached to this task and connect to the IP address "8.8.8.8" on port "1234", and you'll receive a flag.



Lab :-

\----

Step-1 :-

\-------

Here Give command nc 8.8.8.8 1234

Output :-

\------

nc 8.8.8.8 1234

Connection Received: THM{YOU\_CONNECTED\_TO\_A\_PORT}



Step-2 :-

\------

Now we the flag THM{YOU\_CONNECTED\_TO\_A\_PORT} and that's how our this lab is solved.



Answer the questions below:

1. What is the flag received from the challenge?



Answer : THM{YOU\_CONNECTED\_TO\_A\_PORT}

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Extending Your Network Room :-

\---------------------------



Task 1 :-

\-------

Introduction to Port Forwarding :-

\--------------------------------

Port forwarding is an essential component in connecting applications and services to the Internet. Without port forwarding, applications and services such as web servers are only available to devices within the same direct network.



Take the network below as an example. Within this network, the server with an IP address of "192.168.1.10" runs a webserver on port 80. Only the two other computers on this network will be able to access it (this is known as an intranet).



If the administrator wanted the website to be accessible to the public (using the Internet), they would have to implement port forwarding, Network #2 will now be able to access the webserver running on Network #1 using the public IP address of Network #1 (82.62.51.70).



It is easy to confuse port forwarding with the behaviours of a firewall (a technology we'll come on to discuss in a later task). However, at this stage, just understand that port forwarding opens specific ports (recall how packets work). In comparison, firewalls determine if traffic can travel across these ports (even if these ports are open by port forwarding).



Port forwarding is configured at the router of a network.



Answer the questions below:

What is the name of the device that is used to configure port forwarding?



Answer : router

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Firewalls 101 :-

\-------------

A firewall is a device within a network responsible for determining what traffic is allowed to enter and exit. Think of a firewall as border security for a network. An administrator can configure a firewall to permit or deny traffic from entering or exiting a network based on numerous factors such as:



* Where the traffic is coming from? (has the firewall been told to accept/deny traffic from a specific network?)
* Where is the traffic going to? (has the firewall been told to accept/deny traffic destined for a specific network?)
* What port is the traffic for? (has the firewall been told to accept/deny traffic destined for port 80 only?)
* What protocol is the traffic using? (has the firewall been told to accept/deny traffic that is UDP, TCP or both?)
* Firewalls perform packet inspection to determine the answers to these questions.



Firewalls come in all shapes and sizes. From dedicated pieces of hardware (often found in large networks like businesses) that can handle a magnitude of data to residential routers (like at your home!) or software such as Snort(opens in new tab), firewalls can be categorised into 2 to 5 categories.



We'll cover the two primary categories of firewalls in the table below:



|Firewall Category|Description|
|-|-|
|Stateful|This type of firewall uses the entire information from a connection; rather than inspecting an individual packet, this firewall determines the behaviour of a device based upon the entire connection.<br /><br />This firewall type consumes many resources in comparison to stateless firewalls as the decision making is dynamic. For example, a firewall could allow the first parts of a TCP handshake that would later fail.<br /><br />If a connection from a host is bad, it will block the entire device.|
|Stateless|This firewall type uses a static set of rules to determine whether or not individual packets are acceptable or not. For example, a device sending a bad packet will not necessarily mean that the entire device is then blocked.<br /><br />Whilst these firewalls use much fewer resources than alternatives, they are much dumber. For example, these firewalls are only effective as the rules that are defined within them. If a rule is not exactly matched, it is effectively useless.<br /><br />However, these firewalls are great when receiving large amounts of traffic from a set of hosts (such as a Distributed Denial-of-Service attack)|



Answer the questions below:

What layers of the OSI model do firewalls operate at?



For this answer, just provide the numbers in ascending order, separated by an ampersand (\&) I.e: 4 \& 5



Answer : 3 \& 4

\------



What category of firewall inspects the entire connection?



Answer : stateful

\------



What category of firewall inspects individual packets?



Answer : stateless

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Practical - Firewall :-

\--------------------

Deploy the static site attached to this task.



Malicious traffic are marked as the packets in red. The legitimate traffic are the packets marked green. The protocol you need to block is port 80. Configure the firewall to prevent the malicious packets from reaching the web sever 203.0.110.1.



Lab Scenario :-

\------------

Node A (IP address --- 192.51.100.34) connected to router and that router forward Malicious red traffic to web server (IP address --- 203.0.110.1)

Node B (IP Address --- 203.0.113.99) connected to router and that router forward legitimate traffic to web server (IP address --- 203.0.110.1)

Step-1 :-

\-------

Now add rule where this following we set in router:



|Source IP|Destination IP|Port|Action|
|-|-|-|-|
|198.51.100.34|203.0.110.1|80|DROP|



Step-2 :-

\-------

Now just Node B (IP Address --- 203.0.113.99) connected to router and that router forward legitimate traffic to web server (IP address --- 203.0.110.1) and other side Node A (IP address --- 192.51.100.34) connected to router and that router forward Malicious red traffic to web server (IP address --- 203.0.110.1) is being Dropped by the router before reach to the web server.



Answer the questions below:

What is the flag?



Answer : THM{FIREWALLS\_RULE}

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

VPN Basics :-

\----------

A Virtual Private Network (or VPN for short) is a technology that allows devices on separate networks to communicate securely by creating a dedicated path between each other over the Internet (known as a tunnel). Devices connected within this tunnel form their own private network.



For example, only devices within the same network (such as within a business) can directly communicate. However, a VPN allows two offices to be connected. Let's take the diagram below, where there are three networks:



* Network #1 (Office #1)
* Network #2 (Office #2)
* Network #3 (Two devices connected via a VPN)



The devices connected on Network #3 are still a part of Network #1 and Network #2 but also form together to create a private network (Network #3) that only devices that are connected via this VPN can communicate over.



Let's cover some of the other benefits offered by a VPN in the table below:



|Benefit|Description|
|-|-|
|Allows networks in different geographical locations to be connected.|For example, a business with multiple offices will find VPNs beneficial, as it means that resources like servers/infrastructure can be accessed from another office.|
|Offers privacy.|VPN technology uses encryption to protect data. This means that it can only be understood between the devices it was being sent from and is destined for, meaning the data isn't vulnerable to sniffing.<br /><br />This encryption is useful in places with public WiFi, where no encryption is provided by the network. You can use a VPN to protect your traffic from being viewed by other people.|
|Offers anonymity.|Journalists and activists depend upon VPNs to safely report on global issues in countries where freedom of speech is controlled.<br /><br />Usually, your traffic can be viewed by your ISP and other intermediaries and, therefore, tracked. <br /><br />The level of anonymity a VPN provides is only as much as how other devices on the network respect privacy. For example, a VPN that logs all of your data/history is essentially the same as not using a VPN in this regard.|



TryHackMe uses a VPN to connect you to our vulnerable machines without making them directly accessible on the Internet! This means that:



* You can securely interact with our machines
* Service providers such as ISPs don't think you are attacking another machine on the Internet (which could be against the terms of service)
* The VPN provides security to TryHackMe as vulnerable machines are not accessible using the Internet.



VPN technology has improved over the years. Let's explore some existing VPN technologies below:



|VPN Technology|Description|
|-|-|
|PPP|This technology is used by PPTP (explained below) to allow for authentication and provide encryption of data. VPNs work by using a private key and public certificate (similar to SSH). A private key \& certificate must match for you to connect.<br /><br />This technology is not capable of leaving a network by itself (non-routable).|
|PPTP|The Point-to-Point Tunneling Protocol (PPTP) is the technology that allows the data from PPP to travel and leave a network. <br /><br />PPTP is very easy to set up and is supported by most devices. It is, however, weakly encrypted in comparison to alternatives.|
|IPSec|Internet Protocol Security (IPsec) encrypts data using the existing Internet Protocol (IP) framework.<br /><br />IPSec is difficult to set up in comparison to alternatives; however, if successful, it boasts strong encryption and is also supported on many devices.|



Answer the questions below:

What VPN technology only encrypts \& provides the authentication of data?



Answer : PPP

\------



What VPN technology uses the IP framework?



Answer : IPSec

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\------

LAN Networking Devices :-

\----------------------

What is a Router?

It's a router's job to connect networks and pass data between them. It does this by using routing (hence the name router!).

&#x20;

Routing is the label given to the process of data travelling across networks. Routing involves creating a path between networks so that this data can be successfully delivered. Routers operate at Layer 3 of the OSI model. They often feature an interactive interface (such as a website or a console) that allows an administrator to configure various rules such as port forwarding or firewalling.

&#x20;

Routing is useful when devices are connected by many paths, where the most optimal path is taken:

Routers are dedicated devices and do not perform the same functions as switches.



We can see that Computer A's network is connected to the network of Computer B by two routers in the middle. The question is: what path will be taken? Different protocols will decide what path should be taken, but factors include:



&#x20;



1. &#x20;What path is the shortest?



2\.  What path is the most reliable?



3\.  Which path has the faster medium (e.g. copper or fibre)?



* What is a Switch?



Answer : A switch is a dedicated networking device responsible for providing a means of connecting to multiple devices. Switches can facilitate many devices (from 3 to 63) using Ethernet cables. Switches can operate at both layer 2 and layer 3 of the OSI model. However, these are exclusive in the sense that Layer 2 switches cannot operate at layer 3. Take, for example, a layer 2 switch in the diagram below. These switches will forward frames (remember that the original IP packets are encapsulated within the frames) onto the connected devices using their MAC address.



These switches are solely responsible for sending frames to the correct device.



Now, let's move onto layer 3 switches. These switches are more sophisticated than layer 2, as they can perform some of the responsibilities of a router. Namely, these switches will send frames to devices (as layer 2 does) and route packets to other devices using the IP protocol.



Let's take a look at the diagram below of a layer 3 switch in action. We can see that there are two IP addresses:



192.168.1.1

192.168.2.1

&#x20;

A technology called VLAN (Virtual Local Area Network) allows specific devices within a network to be virtually split up. This split means they can all benefit from things such as an Internet connection but are treated separately. This network separation provides security because it means that rules in place determine how specific devices communicate with each other. This is segregation.



Suppose for example the "Sales Department" and "Accounting Department" will be able to access the Internet, but not able to communicate with each other (although they are connected to the same switch).



Answer the questions below:

1. What is the verb for the action that a router does?



Answer : routing

\------



2\. What are the two different layers of switches? Separate these by a comma I.e.: Layer X,Layer Y



Answer : Layer 2,Layer 3

\-------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 6 :-

\------

Practical - Network Simulator :-

\-----------------------------

Deploy the static site attached to this task. And experiment with the network simulator. The simulator will break down every step a packet needs to take to get from point a to b. Try sending a TCP packet from computer1 to computer3 to reveal a flag.



Lab Scenario :-

\------------

Computer 1 and Computer 2 connected to a switch 1 and switch 1 connected to a router, Now router connected to switch 2 and switch 2 connected to Computer 3.

&#x20;

Step-1 :-

\------

First we Send TCP packet from Computer 1 to Computer 3 Where Computer 1 Send data Hello BOB and we click on send packet.



Step-2 :-

\------

Now under step by step we see what actually happen when Computer 1 send data to Computer 3 -------------



1. HANDSHAKE: Starting TCP/IP Handshake between computer1 and computer3
2. HANDSHAKE: Sending SYN Packet from computer1 to computer3
3. ROUTING: computer1 says computer3 is not on my local network sending to gateway: router
4. ARP REQUEST: Who has router tell computer1
5. ARP RESPONSE: Hey computer1, I am router
6. ARP REQUEST: Who has computer3 tell router
7. ARP RESPONSE: Hey router, I am computer3
8. HANDSHAKE: computer3 received SYN Packet from computer1, sending SYN/ACK Packet to computer1
9. HANDSHAKE: computer1 received SYN/ACK Packet from computer3, sending ACK packet to computer3

10\. HANDSHAKE: computer3 received ACK packet from computer1, Handshake Complete

11\. TCP: Sending TCP packet from computer1 to computer3

12\. TCP: computer3 received TCP Packet from computer1, sending ACK Packet to computer1



Step-3 :-

\------

Now after that data successfully send from Computer 1 to Computer 3 we get pop up and get flag THM{YOU'VE\_GOT\_DATA}.

Answer the questions below:

1. What is the flag from the network simulator?



Answer : THM{YOU'VE\_GOT\_DATA}

\------



How many HANDSHAKE entries are there in the Network Log?



Answer : 5

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

DNS in Detail Room :-

\-------------------



Task 1 :-

\-------

What is DNS? :-

\-------------

What is DNS?

DNS (Domain Name System) provides a simple way for us to communicate with devices on the internet without remembering complex numbers. Much like every house has a unique address for sending mail directly to it, every computer on the internet has its own unique address to communicate with it called an IP address. An IP address looks like the following 104.26.10.229, 4 sets of digits ranging from 0 - 255 separated by a period. When you want to visit a website, it's not exactly convenient to remember this complicated set of numbers, and that's where DNS can help. So instead of remembering 104.26.10.229, you can remember tryhackme.com instead.



Answer the questions below :

What does DNS stand for?



Answer : Domain Name System

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Domain Hierarchy :-

\-----------------

Domain Hierarchy :-

\----------------

A diagram of the domain hierarchy, with the root domain at the top, branching into several top-level domains, which in turn brnach into second level domains



1. TLD (Top-Level Domain) :-

&#x20;  ----------------------

A TLD is the most righthand part of a domain name. So, for example, the tryhackme.com TLD is .com. There are two types of TLD, gTLD (Generic Top Level) and ccTLD (Country Code Top Level Domain). Historically a gTLD was meant to tell the user the domain name's purpose; for example, a .com would be for commercial purposes, .org for an organisation, .edu for education and .gov for government. And a ccTLD was used for geographical purposes, for example, .ca for sites based in Canada, .co.uk for sites based in the United Kingdom and so on. Due to such demand, there is an influx of new gTLDs ranging from .online , .club , .website , .biz and so many more. For a full list of over 2000 TLDs click here(opens in new tab).



2\. Second-Level Domain :-

&#x20;  -------------------

Taking tryhackme.com as an example, the .com part is the TLD, and tryhackme is the Second Level Domain. When registering a domain name, the second-level domain is limited to 63 characters + the TLD and can only use a-z 0-9 and hyphens (cannot start or end with hyphens or have consecutive hyphens).



3\. Subdomain :-

&#x20;  ---------

A subdomain sits on the left-hand side of the Second-Level Domain using a period to separate it; for example, in the name admin.tryhackme.com the admin part is the subdomain. A subdomain name has the same creation restrictions as a Second-Level Domain, being limited to 63 characters and can only use a-z 0-9 and hyphens (cannot start or end with hyphens or have consecutive hyphens). You can use multiple subdomains split with periods to create longer names, such as jupiter.servers.tryhackme.com. But the length must be kept to 253 characters or less. There is no limit to the number of subdomains you can create for your domain name.



Answer the questions below:

1. What is the maximum length of a subdomain?



Answer : 63

\------



2\. Which of the following characters cannot be used in a subdomain ( 3 b \_ - )?



Answer : \_

\------



3\. What is the maximum length of a domain name?



Answer : 253

\------



4\. What type of TLD is .co.uk?



Answer : ccTLD

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Record Types :-

\------------



DNS Record Types :-

\----------------

DNS isn't just for websites though, and multiple types of DNS record exist. We'll go over some of the most common ones that you're likely to come across.



A Record :-

\--------

These records resolve to IPv4 addresses, for example 104.26.10.229



AAAA Record :-

\-----------

These records resolve to IPv6 addresses, for example 2606:4700:20::681a:be5



CNAME Record :-

\------------

These records resolve to another domain name, for example, TryHackMe's online shop has the subdomain name store.tryhackme.com which returns a CNAME record shops.shopify.com(opens in new tab). Another DNS request would then be made to shops.shopify.com(opens in new tab) to work out the IP address.



MX Record :-

\---------

These records resolve to the address of the servers that handle the email for the domain you are querying, for example an MX record response for tryhackme.com would look something like alt1.aspmx.l.google.com(opens in new tab). These records also come with a priority flag. This tells the client in which order to try the servers, this is perfect for if the main server goes down and email needs to be sent to a backup server.



TXT Record :-

\-----------

TXT records are free text fields where any text-based data can be stored. TXT records have multiple uses, but some common ones can be to list servers that have the authority to send an email on behalf of the domain (this can help in the battle against spam and spoofed email). They can also be used to verify ownership of the domain name when signing up for third party services. Here are a few examples:



* \_acme-challenge.example.com TXT "token\_value\_here"
* @ TXT "v=spf1 ip4:192.0.2.0/24 include:\_spf.google.com include:amazonses.com \~all"
* \_dmarc.example.com TXT "v=DMARC1; p=reject; rua=mailto:dmarc-reports@example.com; adkim=s; aspf=s; pct=100"
* @ TXT "MS=ms12345678"



As you can see, as the name implies, TXT records are strings of text.



Answer the questions below:

1. What type of record would be used to advise where to send email?



Answer : MX

\------



2\. What type of record handles IPv6 addresses?



Answer : AAAA

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Making A Request :-

\----------------



What happens when you make a DNS request :-

\----------------------------------------

a diagram visualizing the flow described in the text ----------



1. When you request a domain name, your computer first checks its local cache to see if you've previously looked up the address recently; if not, a request to your Recursive DNS Server will be made.



2\. A Recursive DNS Server is usually provided by your ISP, but you can also choose your own. This server also has a local cache of recently looked up domain names. If a result is found locally, this is sent back to your computer, and your request ends here (this is common for popular and heavily requested services such as Google, Facebook, Twitter). If the request cannot be found locally, a journey begins to find the correct answer, starting with the internet's root DNS servers.



3\. The root servers act as the DNS backbone of the internet; their job is to redirect you to the correct Top Level Domain Server, depending on your request. If, for example, you request www.tryhackme.com, the root server will recognise the Top Level Domain of .com and refer you to the correct TLD server that deals with .com addresses.



4\. The TLD server holds records for where to find the authoritative server to answer the DNS request. The authoritative server is often also known as the nameserver for the domain. For example, the name server for tryhackme.com is kip.ns.cloudflare.com(opens in new tab) and uma.ns.cloudflare.com(opens in new tab). You'll often find multiple nameservers for a domain name to act as a backup in case one goes down.



5\. An authoritative DNS server is the server that is responsible for storing the DNS records for a particular domain name and where any updates to your domain name DNS records would be made. Depending on the record type, the DNS record is then sent back to the Recursive DNS Server, where a local copy will be cached for future requests and then relayed back to the original client that made the request. DNS records all come with a TTL (Time To Live) value. This value is a number represented in seconds that the response should be saved for locally until you have to look it up again. Caching saves on having to make a DNS request every time you communicate with a server.



Answer the questions below:

1. What field specifies how long a DNS record should be cached for?



Answer : TTL

\------



2\. What type of DNS Server is usually provided by your ISP?



Answer : recursive

\------



What type of server holds all the records for a domain?



Answer : authoritative

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\-------

Practical :-

\---------

Using the website on the right, we can build requests to make DNS queries and view the results. The website will also show you the command you'd need to run on your own computer if you wished to make the requests yourself.



Lab :-

\---

Step-1 :-

\------

First we set the DNS type CNAME and then give subdomain shop and click on Send DNS request.



Step-2 :-

\------

After that our command finally become nslookup --type=CNAME shop.website.thm



Output :-

\------

user@thm:\~$ nslookup --type=CNAME shop.website.thm

Server: 127.0.0.53

Address: 127.0.0.53#53



Non-authoritative answer:

shop.website.thm canonical name = shops.myshopify.com



Step-3 :-

\------

Now we get shop.website.thm canonical name shops.myshopify.com



Step-4 :-

\------

Now that's how we get 1st question answer.



Step-5 :-

\------

Now we choose the DNS type txt and click on send DNS request.



Step-6 :-

\------

After that our command finally become nslookup --type=TXT website.thm



Output :-

\------

user@thm:\~$ nslookup --type=TXT website.thm

Server: 127.0.0.53

Address: 127.0.0.53#53



Non-authoritative answer:

website.thm text = "THM{7012BBA60997F35A9516C2E16D2944FF}"



Step-7 :-

\------

Now that's how we get txt record THM{7012BBA60997F35A9516C2E16D2944FF}



Step-8 :-

\------

Now we that's how we solve the 2nd question answer



Step-9 :-

\------

Now we choose the DNS type MX and click on Send DNS request



Step-10 :-

\-------

Now we set our command nslookup --type=MX website.thm



Output :-

\------

user@thm:\~$ nslookup --type=MX website.thm

Server: 127.0.0.53

Address: 127.0.0.53#53



Non-authoritative answer:

website.thm mail exchanger = 30 alt4.aspmx.l.google.com



Step-11 :-

\-------

Now we get the priority value of MX record 30 at first



Step-12 :-

\-------

Now that's how we solve the 3rd question answer.



Step-13 :-

\-------

Now we choose the DNS type A and click on Send DNS request



Step-14 :-

\-------

Now we set our command nslookup --type=A website.thm



Output :-

\------

user@thm:\~$ nslookup --type=A website.thm

Server: 127.0.0.53

Address: 127.0.0.53#53



Non-authoritative answer:

Name: website.thm

Address: 10.10.10.10



Step-15 :-

\-------

Now we get the IP address of the website.thm which we see is 10.10.10.10



Step-16 :-

\-------

Now that's how we solve the 4th and final question answer.





Answer the questions below:

1. What is the CNAME of shop.website.thm?



Answer : shops.myshopify.com

\------



2\. What is the value of the TXT record of website.thm?



Answer : THM{7012BBA60997F35A9516C2E16D2944FF}

\------



3\. What is the numerical priority value for the MX record?



Answer : 30

\------



4\. What is the IP address for the A record of www.website.thm?



Answer : 10.10.10.10

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

HTTP in Detail Room :-

\-------------------



Task 1 :-

\------

What is HTTP(S)? :-

\----------------



What is HTTP? (HyperText Transfer Protocol)



Answer : HTTP is what's used whenever you view a website, developed by Tim Berners-Lee and his team between 1989-1991. HTTP is the set of rules used for communicating with web servers for the transmitting of webpage data, whether that is HTML, Images, Videos, etc.



What is HTTPS? (HyperText Transfer Protocol Secure)



Answer : HTTPS is the secure version of HTTP. HTTPS data is encrypted so it not only stops people from seeing the data you are receiving and sending, but it also gives you assurances that you're talking to the correct web server and not something impersonating it.



Lab :-

\----

Step-1 :-

\------

Here when open the webpage there we see a problem that is it run on http like http://tryhackme.com/ and It's HTTP certificate is invalid.



Step-2 :-

\------

So now it run in http so it is not secure to see its http cert we click on the not secure lock image and the flag THM{INVALID\_HTTP\_CERT}is show in pop up in our browser and thats how our 3rd number question is solved.



Answer the questions below:

1. What does HTTP stand for?



Answer : HyperText Transfer Protocol

\------



2\. What does the S in HTTPS stand for?



Answer : secure

\------



3\. On the mock webpage on the right there is an issue, once you've found it, click on it. What is the challenge flag?



Answer : THM{INVALID\_HTTP\_CERT}

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

Requests And Responses :-

\----------------------

When we access a website, your browser will need to make requests to a web server for assets such as HTML, Images, and download the responses. Before that, you need to tell the browser specifically how and where to access these resources, this is where URLs will help.



1. What is a URL? (Uniform Resource Locator)



Answer : If you’ve used the internet, you’ve used a URL before. A URL is predominantly an instruction on how to access a resource on the internet. The below image shows what a URL looks like with all of its features (it does not use all features in every request).



A diagram showing different parts of a URL on an example, where http is the scheme, user:password is the user, tryhackme.com is a domain or the host, 80 is the port, view-room is the path, ?id=1 is the query string, and #task3 is the fragment. The full address is http://user:password@tryhackme.com:80/view-room?id=1#task3.



* Scheme: This instructs on what protocol to use for accessing the resource such as HTTP, HTTPS, FTP (File Transfer Protocol).



* User: Some services require authentication to log in, you can put a username and password into the URL to log in.



* Host: The domain name or IP address of the server you wish to access.



* Port: The Port that you are going to connect to, usually 80 for HTTP and 443 for HTTPS, but this can be hosted on any port between 1 - 65535.



* Path: The file name or location of the resource you are trying to access.



* Query String: Extra bits of information that can be sent to the requested path. For example, /blog?id=1 would tell the blog path that you wish to receive the blog article with the id of 1.



Fragment: This is a reference to a location on the actual page requested. This is commonly used for pages with long content and can have a certain part of the page directly linked to it, so it is viewable to the user as soon as they access the page.



1. Making a Request :-

&#x20;  -----------------

It's possible to make a request to a web server with just one line GET / HTTP/1.1



But for a much richer web experience, you’ll need to send other data as well. This other data is sent in what is called headers, where headers contain extra information to give to the web server you’re communicating with, but we’ll go more into this in the Header task.



Example Request :-

\---------------

GET / HTTP/1.1



* Host: tryhackme.com
* User-Agent: Mozilla/5.0 Firefox/87.0
* Referer: https://tryhackme.com/



To breakdown each line of this request :-

\--------------------------------------

* Line 1: This request is sending the GET method ( more on this in the HTTP Methods task ), request the home page with / and telling the web server we are using HTTP protocol version 1.1.



* Line 2: We tell the web server we want the website tryhackme.com



* Line 3: We tell the web server we are using the Firefox version 87 Browser



* Line 4: We are telling the web server that the web page that referred us to this one is https://tryhackme.com



* Line 5: HTTP requests always end with a blank line to inform the web server that the request has finished.



Example Response :-

\----------------

HTTP/1.1 200 OK



* Server: nginx/1.15.8
* Date: Fri, 09 Apr 2021 13:34:03 GMT
* Content-Type: text/html
* Content-Length: 98



<html>

<head>

&#x20;   <title>TryHackMe</title>

</head>

<body>

&#x20;   Welcome To TryHackMe.com

</body>

</html>



To breakdown each line of the response :-

\---------------------------------------

* Line 1: HTTP 1.1 is the version of the HTTP protocol the server is using and then followed by the HTTP Status Code in this case "200 OK" which tells us the request has completed successfully.



* Line 2: This tells us the web server software and version number.



* Line 3: The current date, time and timezone of the web server.



* Line 4: The Content-Type header tells the client what sort of information is going to be sent, such as HTML, images, videos, pdf, XML.



* Line 5: Content-Length tells the client how long the response is, this way we can confirm no data is missing.



* Line 6: HTTP response contains a blank line to confirm the end of the HTTP response.



* Lines 7-14: The information that has been requested, in this instance the homepage.



Answer the questions below:

1. What HTTP protocol is being used in the above example?



Answer : HTTP/1.1

\-------



2\. What response header tells the browser how much data to expect?



Answer : Content-Length

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

HTTP Methods :-

\------------

HTTP methods are a way for the client to show their intended action when making an HTTP request. There are a lot of HTTP methods but we'll cover the most common ones, although mostly you'll deal with the GET and POST method.



1. GET Request :-

&#x20;  ------------

This is used for getting information from a web server.



2\. POST Request :-

&#x20;  ------------

This is used for submitting data to the web server and potentially creating new records



3\. PUT Request :-

&#x20;  -----------

This is used for submitting data to a web server to update information



4\. DELETE Request :-

&#x20;  --------------

This is used for deleting information/records from a web server.



Answer the questions below:

What method would be used to create a new user account?



Answer : POST

\------



What method would be used to update your email address?



Answer : PUT

\------



What method would be used to remove a picture you've uploaded to your account?



Answer : DELETE

\------



What method would be used to view a news article?



Answer : GET

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

HTTP Status Codes :-

\-----------------



HTTP Status Codes :-

\-----------------

In the previous task, you learnt that when a HTTP server responds, the first line always contains a status code informing the client of the outcome of their request and also potentially how to handle it. These status codes can be broken down into 5 different ranges:



|100-199 - Information Response|These are sent to tell the client the first part of their request has been accepted and they should continue sending the rest of their request. These codes are no longer very common.|
|-|-|
|200-299 - Success|This range of status codes is used to tell the client their request was successful.|
|300-399 - Redirection|These are used to redirect the client's request to another resource. This can be either to a different webpage or a different website altogether.|
|400-499 - Client Errors|Used to inform the client that there was an error with their request.|
|500-599 - Server Errors|This is reserved for errors happening on the server-side and usually indicate quite a major problem with the server handling the request.|



Common HTTP Status Codes :-

\------------------------

There are a lot of different HTTP status codes and that's not including the fact that applications can even define their own, we'll go over the most common HTTP responses you are likely to come across:



|200 - OK|The request was completed successfully.|
|-|-|
|201 - Created|A resource has been created (for example a new user or new blog post).|
|301 - Moved Permanently|This redirects the client's browser to a new webpage or tells search engines that the page has moved somewhere else and to look there instead.|
|302 - Found|Similar to the above permanent redirect, but as the name suggests, this is only a temporary change and it may change again in the near future.|
|400 - Bad Request|This tells the browser that something was either wrong or missing in their request. This could sometimes be used if the web server resource that is being requested expected a certain parameter that the client didn't send.|
|401 - Not Authorised|You are not currently allowed to view this resource until you have authorised with the web application, most commonly with a username and password.|
|403 - Forbidden|You do not have permission to view this resource whether you are logged in or not.|
|405 - Method Not Allowed|The resource does not allow this method request, for example, you send a GET request to the resource /create-account when it was expecting a POST request instead.|
|404 - Page Not Found|The page/resource you requested does not exist.|
|500 - Internal Service Error|The server has encountered some kind of error with your request that it doesn't know how to handle properly.|
|503 - Service Unavailable|This server cannot handle your request as it's either overloaded or down for maintenance.|



Answer the questions below:

1. What response code might you receive if you've created a new user or blog post article?



Answer : 201

\------



2\. What response code might you receive if you've tried to access a page that doesn't exist?



Answer : 404

\------



3\. What response code might you receive if the web server cannot access its database and the application crashes?



Answer : 503

\------



4\. What response code might you receive if you try to edit your profile without logging in first?



Answer : 401

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\------

Headers :-

\-------

Headers are additional bits of data you can send to the web server when making requests.

Although no headers are strictly required when making a HTTP request, you’ll find it difficult to view a website properly.



Common Request Headers :-

\----------------------

﻿These are headers that are sent from the client (usually your browser) to the server.



* Host: Some web servers host multiple websites so by providing the host headers you can tell it which one you require, otherwise you'll just receive the default website for the server.



* User-Agent: This is your browser software and version number, telling the web server your browser software helps it format the website properly for your browser and also some elements of HTML, JavaScript and CSS are only available in certain browsers.



* Content-Length: When sending data to a web server such as in a form, the content length tells the web server how much data to expect in the web request. This way the server can ensure it isn't missing any data.



* Accept-Encoding: Tells the web server what types of compression methods the browser supports so the data can be made smaller for transmitting over the internet.





* Cookie: Data sent to the server to help remember your information (see cookies task for more information).

Common Response Headers





These are the headers that are returned to the client from the server after a request.



* Set-Cookie: Information to store which gets sent back to the web server on each request (see cookies task for more information).



* Cache-Control: How long to store the content of the response in the browser's cache before it requests it again.



* Content-Type: This tells the client what type of data is being returned, i.e., HTML, CSS, JavaScript, Images, PDF, Video, etc. Using the content-type header the browser then knows how to process the data.



* Content-Encoding: What method has been used to compress the data to make it smaller when sending it over the internet.



Answer the questions below:

What header tells the web server what browser is being used?



Answer : User-Agent

\------



What header tells the browser what type of data is being returned?



Answer : Content-Type

\------



What header tells the web server which website is being requested?



Answer : Host

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 6 :-

\-------

Cookies :-

\-------

You've probably heard of cookies before, they're just a small piece of data that is stored on your computer. Cookies are saved when you receive a "Set-Cookie" header from a web server. Then every further request you make, you'll send the cookie data back to the web server. Because HTTP is stateless (doesn't keep track of your previous requests), cookies can be used to remind the web server who you are, some personal settings for the website or whether you've been to the website before. Let's take a look at this as an example HTTP request:



Cookies can be used for many purposes but are most commonly used for website authentication. The cookie value won't usually be a clear-text string where you can see the password, but a token (unique secret code that isn't easily humanly guessable).



Viewing Your Cookies :-

\--------------------

You can easily view what cookies your browser is sending to a website by using the developer tools, in your browser. If you're not sure how to get to the developer tools in your browser, click on the "View Site" button at the top of this task for a how-to guide.



Once you have developer tools open, click on the "Network" tab. This tab will show you a list of all the resources your browser has requested. You can click on each one to receive a detailed breakdown of the request and response. If your browser sent a cookie, you will see these on the "Cookies" tab of the request.



To see the cookies in developers Tools in different browser we follow the following process:

1. Firefox :-

&#x20;  --------

To open the developer tools in Firefox, click the Firefox Menu icon on the top right of the browser. Then, select More tools. In the submenu, choose Web Developer Tools.



2\. Chrome :-

&#x20;  ------

To open the developer tools in Chrome, click the Chrome Menu icon on the top right of the browser. Then, select More Tools. In the submenu, choose Developer Tools.



3\. Safari :-

&#x20;  ------

To open the developer tools in Safari, first enable the Developer Menu. Click Safari Menu > Settings to open the settings and preferences panel in Safari.



4\. Edge :-

&#x20; ------

To open the developer tools in Microsoft Edge, click on the Edge Menu on the right-hand side of the browser and then select More tools. From the submenu, select Developer Tools.



5\. Internet Explorer :-

&#x20;  -----------------

To open the developer tools in Internet Explorer, click on the cog menu icon on the right-hand side of the browser and then select F12 Developer Tools.



Answer the questions below:

Which header is used to save cookies to your computer?



Answer : Set-Cookie

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 7

Making Requests :-

\---------------

This is an emulator for making demo HTTP requests, using what you've learnt from the above tasks you can use it to complete the below questions.



Lab :-

\---

Step-1 :-

\------

First we set the request type GET and give URL http://tryhackme.com/room and click on Go



Request :-

\--------

GET /room HTTP/1.1



Host: tryhackme.com



User-Agent: Mozilla/5.0 Firefox/87.0



Content-Length: 0



Response :-

\--------

HTTP/1.1 200 Ok

Server: nginx/1.15.8

Wed, 9 Sep 2026 20:58:2 GMT

Content-Type: text/html; charset=utf-8

Content-Length: 252

Last-Modified: Wed, 9 Sep 2026 20:58:2 GMT



<html>

<head>

&#x20;   <title>TryHackMe</title>

</head>

<body>

&#x20;   Welcome to the Room page THM{YOU'RE\_IN\_THE\_ROOM}

</body>

</html>



THM Browser :-

\-----------

Welcome to the Room page THM{YOU'RE\_IN\_THE\_ROOM}



Step-2 :-

\-------

Now we set the Request type GET and URL http://tryhackme.com/blog?id=1 and click on Go



Request :-

\-------

GET /blog?id=1 HTTP/1.1



Host: tryhackme.com



User-Agent: Mozilla/5.0 Firefox/87.0



Content-Length: 0



Response :-

\--------

HTTP/1.1 200 Ok

Server: nginx/1.15.8

Wed, 9 Sep 2026 21:4:51 GMT

Content-Type: text/html; charset=utf-8

Content-Length: 250

Last-Modified: Wed, 9 Sep 2026 21:4:51 GMT



<html>

<head>

&#x20;   <title>TryHackMe</title>

</head>

<body>

&#x20;   Viewing Blog article 1 THM{YOU\_FOUND\_THE\_BLOG}

</body>

</html>



THM Browser :-

\-----------

Viewing Blog article 1 THM{YOU\_FOUND\_THE\_BLOG}



Step-3 :-

\------

Now we set the DELETE request and Give URL http://tryhackme.com/user/1 and click on Go



Request :-

\-------

DELETE /user/1 HTTP/1.1



Host: tryhackme.com



User-Agent: Mozilla/5.0 Firefox/87.0



Content-Length: 0



Response :-

\--------

HTTP/1.1 200 Ok

Server: nginx/1.15.8

Wed, 9 Sep 2026 21:9:53 GMT

Content-Type: text/html; charset=utf-8

Content-Length: 250

Last-Modified: Wed, 9 Sep 2026 21:9:53 GMT



<html>

<head>

&#x20;   <title>TryHackMe</title>

</head>

<body>

&#x20;   The user has been deleted THM{USER\_IS\_DELETED}

</body>

</html>



THM Browser :-

\-----------

The user has been deleted THM{USER\_IS\_DELETED}



Step-4 :-

\-------

Now set PUT request and set URL http://tryhackme.com/user/2?username=admin and click on Go



Request :-

\-------

PUT /user/2 HTTP/1.1



Host: tryhackme.com



User-Agent: Mozilla/5.0 Firefox/87.0



Content-Length: 14



Content-Type: application/x-www-form-urlencoded





username=admin



Response :-

\--------

HTTP/1.1 200 Ok

Server: nginx/1.15.8

Wed, 9 Sep 2026 21:19:30 GMT

Content-Type: text/html; charset=utf-8

Content-Length: 251

Last-Modified: Wed, 9 Sep 2026 21:19:30 GMT



<html>

<head>

&#x20;   <title>TryHackMe</title>

</head>

<body>

&#x20;   Username changed to admin THM{USER\_HAS\_UPDATED}

</body>

</html>



THM Browser :-

\-----------

Username changed to admin THM{USER\_HAS\_UPDATED}



Step-5 :-

\------

Now we set request POST and Give URL http://tryhackme.com/login?username=thm\&password=letmein



Request :-

\-------

POST /login?username=thm\&password=letmein HTTP/1.1



Host: tryhackme.com



User-Agent: Mozilla/5.0 Firefox/87.0



Content-Length: 29



Content-Type: application/x-www-form-urlencoded





username=thm\&password=letmein



Response :-

\--------

HTTP/1.1 200 Ok

Server: nginx/1.15.8

Wed, 9 Sep 2026 21:24:30 GMT

Content-Type: text/html; charset=utf-8

Content-Length: 256

Last-Modified: Wed, 9 Sep 2026 21:24:30 GMT



<html>

<head>

&#x20;   <title>TryHackMe</title>

</head>

<body>

&#x20;   You logged in! Welcome Back THM{HTTP\_REQUEST\_MASTER}

</body>

</html>



THM Browser :-

\-----------

You logged in! Welcome Back THM{HTTP\_REQUEST\_MASTER}



Answer the questions below:

1. Make a GET request to /room page



Answer : THM{YOU'RE\_IN\_THE\_ROOM}

\------



2\. Make a GET request to /blog page and set the id parameter to 1

Note: Use the gear button on the right to manage URI parameters



Answer : THM{YOU\_FOUND\_THE\_BLOG}

\------



3\. Make a DELETE request to /user/1 page



Answer : THM{USER\_IS\_DELETED}

\------



4\. Make a PUT request to /user/2 page with the username parameter set to admin

Note: Use the gear button on the right to manage body parameters



Answer : THM{USER\_HAS\_UPDATED}

\------



5\. Make a POST request to /login page with the username of thm and a password of letmein

Note: Use the gear button on the right to manage body parameters



Answer : THM{HTTP\_REQUEST\_MASTER}

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

How Websites Work Room :-

\----------------------

Task 1 :-

\------

How websites work :-

\-----------------

When you visit a website, your browser (like Safari or Google Chrome) makes a request to a web server asking for information about the page you're visiting. It will respond with data that your browser uses to show you the page; a web server is just a dedicated computer somewhere else in the world that handles your requests.



There are two major components that make up a website:



* Front End (Client-Side) - the way your browser renders a website.
* Back End (Server-Side) - a server that processes your request and returns a response.



There are many other processes involved in your browser making a request to a web server, but for now, you just need to understand that you make a request to a server, and it responds with data your browser uses to render information to you.



Answer the questions below:

What term best describes the component of a web application rendered by your browser?



Answer : Front End

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

HTML :-

\----

Websites are primarily created using:



* HTML, to build websites and define their structure
* CSS, to make websites look pretty by adding styling options
* JavaScript, implement complex features on pages using interactivity
* HyperText Markup Language (HTML) is the language websites are written in. Elements (also known as tags) are the building blocks of HTML pages and tells the browser how to display content. The code snippet below shows a simple HTML document, the structure of which is the same for every website:





The HTML structure (as shown in the screenshot) has the following components:



* The <!DOCTYPE html> defines that the page is a HTML5 document. This helps with standardisation across different browsers and tells the browser to use HTML5 to interpret the page.
* The <html> element is the root element of the HTML page - all other elements come after this element.
* The <head> element contains information about the page (such as the page title)
* The <body> element defines the HTML document's body; only content inside of the body is shown in the browser.
* The <h1> element defines a large heading
* The <p> element defines a paragraph



There are many other elements (tags) used for different purposes. For example, there are tags for buttons (<button>), images (<img>), lists, and much more.

Tags can contain attributes such as the class attribute which can be used to style an element (e.g. make the tag a different color) <p class="bold-text">, or the src attribute which is used on images to specify the location of an image: <img src="img/cat.jpg">.An element can have multiple attributes each with its own unique purpose, e.g., <p attribute1="value1" attribute2="value2">.



Elements can also have an id attribute (<p id="example">), which is unique to the element. Unlike the class attribute, where multiple elements can use the same class, an element must have different id's to identify them uniquely. Element id's are used for styling and to identify it by JavaScript.



You can view the HTML of any website by right-clicking and selecting "View Page Source" (Chrome) / "Show Page Source" (Safari).



Lab :-

\---

Step-1 :-

\------

Under we see two image after rendering of cat one picture or image is correctly render and show the image in Front end and other not show there is a issue that after when we solve then the second picture is show.



Code :-

\----

<!DOCTYPE html>

<html>

&#x20;   <head>

&#x20;       <title>TryHackMe HTML Editor</title>

&#x20;   </head>

&#x20;   <body>

&#x20;       <h1>Cat Website!</h1>

&#x20;       <p>See images of all my cats!</p>

&#x20;       <img src='img/cat-1.jpg'>

&#x20;       <img src='img/cat-2.'>

&#x20;       <!-- Add dog image here -->

&#x20;   </body>

</html>



Step-2 :-

\------

So here we see that . then in cat-2 the jpg extension not given so it not fount the cat-2.jpg image and render it in client side so we just put the .jpg extension in beside of the cat-2 and then we see that our second cat image in Front end correctly render and show on which our secret code is written HTMLHERO that we copy and paste in 2nd question answer and that's how it become solved.



Code :-

\----

<!DOCTYPE html>

<html>

&#x20;   <head>

&#x20;       <title>TryHackMe HTML Editor</title>

&#x20;   </head>

&#x20;   <body>

&#x20;       <h1>Cat Website!</h1>

&#x20;       <p>See images of all my cats!</p>

&#x20;       <img src='img/cat-1.jpg'>

&#x20;       <img src='img/cat-2.jpg'>

&#x20;       <!-- Add dog image here -->

&#x20;   </body>

</html>



Step-3 :-

\------

Now we third question we have the dog image location in img/dog-1.png and tell that add the dog image code in 11 th line which is this line <!-- Add dog image here -->. We simply replace it by the code and see the dog image is show or not.



Step-4 :-

\------

After written the following code we see dog image appear and correctly render in front end side on which the secret word is written that DOGHTML and it is our secret word and 3rd question want and we give it as third question answer and that's how our third question is solved.



Code :-

\----

<!DOCTYPE html>

<html>

&#x20;   <head>

&#x20;       <title>TryHackMe HTML Editor</title>

&#x20;   </head>

&#x20;   <body>

&#x20;       <h1>Cat Website!</h1>

&#x20;       <p>See images of all my cats!</p>

&#x20;       <img src='img/cat-1.jpg'>

&#x20;       <img src='img/cat-2.jpg'>

&#x20;       <img src=' img/dog-1.png'>

&#x20;   </body>

</html>



Answer the questions below:

1. Let's play with some HTML! First click the "View Site" button inside this task. On the right-hand side, you should see a box that renders HTML - If you enter some HTML into the box and click the green "Render HTML Code" button, it will render your HTML on the page; you should see an image of some cats.



Answer : No answer needed

\------



2\. One of the images on the cat website is broken - fix it, and the image will reveal the hidden text answer!



Answer : HTMLHERO

\------



3\. Add a dog image to the page by adding another img tag (<img>) on line 11. The dog image location is img/dog-1.png. What is the text in the dog image?



Answer : DOGHTML

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

JavaScript :-

\----------

JavaScript (JS) is one of the most popular coding languages in the world and allows pages to become interactive. HTML is used to create the website structure and content, while JavaScript is used to control the functionality of web pages - without JavaScript, a page would not have interactive elements and would always be static. JS can dynamically update the page in real-time, giving functionality to change the style of a button when a particular event on the page occurs (such as when a user clicks a button) or to display moving animations.



JavaScript is added within the page source code and can be either loaded within <script> tags or can be included remotely with the src attribute: <script src="/location/of/javascript\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\_file.js"></script>



The following JavaScript code finds a HTML element on the page with the id of "demo" and changes the element's contents to "Hack the Planet" : document.getElementById("demo").innerHTML = "Hack the Planet";



HTML elements can also have events, such as "onclick" or "onhover" that execute JavaScript when the event occurs. The following code changes the text of the element with the demo ID to Button Clicked: <button onclick='document.getElementById("demo").innerHTML = "Button Clicked";'>Click Me!</button> - onclick events can also be defined inside the JavaScript script tags, and not on elements directly.



Lab :-

\---

Step-1 :-

\-----

Here we see the code that is ----



code :-

\----

<!DOCTYPE html>

<html>

&#x20;   <head>

&#x20;       <title>TryHackMe Editor</title>

&#x20;   </head>

&#x20;   <body>

&#x20;       <div id="demo">Hi there!</div>

&#x20;       <script type="text/javascript">

&#x20;           // add your JavaScript here

&#x20;       </script>

&#x20;   </body>

</html>



Step-2 :-

\------

Now to set demo element's content to "Hack the Planet" we write the code document.getElementById("demo").innerHTML = "Hack the Planet"; under <script type="text/javascript"> so our final code become -----



Code :-

\----

<!DOCTYPE html>

<html>

&#x20;   <head>

&#x20;       <title>TryHackMe Editor</title>

&#x20;   </head>

&#x20;   <body>

&#x20;       <div id="demo">Hi there!</div>

&#x20;       <script type="text/javascript">

&#x20;           document.getElementById("demo").innerHTML = "Hack the Planet";

&#x20;       </script>

&#x20;   </body>

</html>



Step-3 :-

\------

Now we click on Reneder HTML + JS code and see the output in under ----



Rendered HTML Code :-

\------------------

Hack the Planet



Step-4 :-

\------

Now we see that one popup show and there the 1st question answer show JSISFUN

&#x20;

Answer the questions below:

1. Click the "View Site" button on this task. On the right-hand side, add JavaScript that changes the demo element's content to "Hack the Planet"



Answer : JSISFUN

\------



2\. Add the button HTML from this task that changes the element's text to "Button Clicked" on the editor on the right, update the code by clicking the "Render HTML+JS Code" button and then click the button.



Answer : No answer needed

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Sensitive Data Exposure :-

\-----------------------

Sensitive Data Exposure occurs when a website doesn't properly protect (or remove) sensitive clear-text information to the end-user; usually found in a site's frontend source code.



We now know that websites are built using many HTML elements (tags), all of which we can see simply by "viewing the page source". A website developer may have forgotten to remove login credentials, hidden links to private parts of the website or other sensitive data shown in HTML or JavaScript.



Sensitive information can be potentially leveraged to further an attacker's access within different parts of a web application. For example, there could be HTML comments with temporary login credentials, and if you viewed the page's source code and found this, you could use these credentials to log in elsewhere on the application (or worse, used to access other backend components of the site).



Whenever you're assessing a web application for security issues, one of the first things you should do is review the page source code to see if you can find any exposed login credentials or hidden links.



Lab :-

\---

Step-1 :-

\------

we see a frontend webpage where username and password field is present but we don't know that what the username and password is so we first go inspect mode and try to see the source code and in source code try to find the username and password is present or not.



Step-2 :-

\------

Now here we find username and password of admin is hardcoded and it show in the code where written ----



TODO: Remove test credentials!

Username : admin

Password : testpasswd



step-3 :-

\------

Now we click on login button and popup show with congratulations! And we found the password testpasswd and write it as the 1st question answer and that's how our 1st question is solved.



Answer the questions below:

View the website on this link (opens in new tab). What is the password hidden in the source code?



Answer : testpasswd

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 5 :-

\------

HTML Injection :-

\--------------

HTML Injection is a vulnerability that occurs when unfiltered user input is displayed on the page. If a website fails to sanitise user input (filter any "malicious" text that a user inputs into a website), and that input is used on the page, an attacker can inject HTML code into a vulnerable website.



Input sanitisation is very important in keeping a website secure, as information a user inputs into a website is often used in other frontend and backend functionality. A vulnerability you'll explore in another lab is database injection, where you can manipulate a database lookup query to log in as another user by controlling the input that's directly used in the query - but for now, let's focus on HTML injection (which is client-side).



When a user has control of how their input is displayed, they can submit HTML (or JavaScript) code, and the browser will use it on the page, allowing the user to control the page's appearance and functionality.



The image above shows how a form outputs text to the page. Whatever the user inputs into the "What's your name" field is passed to a JavaScript function and output to the page, which means if the user adds their own HTML or JavaScript in the field, it's used in the sayHi function and is added to the page - this means you can add your own HTML (such as a <h1> tag) and it will output your input as pure HTML.



The general rule is never to trust user input. To prevent malicious input, the website developer should sanitise everything the user enters before using it in the JavaScript function; in this case, the developer could remove any HTML tags.



Lab :-

\----

Step-1 :-

\------

First we see a input box that is tell what's your Name and there we put this <a href=http://hacker.com>http://hacker.com</a>



Step-2 :-

\------

Now we when click on Say Hi button then the popup show in browser and there we see that HTML\_INJ3CTI0N as a answer and that's how our 1st question answer is solved.



Answer the questions below:

View the website on this task and inject HTML so that a malicious link to http://hacker.com is shown.



Answer : HTML\_INJ3CTI0N

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Putting it all together Room :-

\----------------------------



Task 1 :-

\------

Putting It All Together :-

\------------------------

From the previous modules, you'll have learned that quite a lot of things go on behind the scenes when you request a webpage in your browser.



To summarise, when you request a website, your computer needs to know the server's IP address it needs to talk to; for this, it uses DNS. Your computer then talks to the web server using a special set of commands called the HTTP protocol; the webserver then returns HTML, JavaScript, CSS, Images, etc., which your browser then uses to correctly format and display the website to you.



There are also a few other components that help the web run more efficiently and provide extra features.



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Other Components :-

\-----------------



1. Load Balancers :-

&#x20;  ---------------

When a website's traffic starts getting quite large or is running an application that needs to have high availability, one web server might no longer do the job. Load balancers provide two main features, ensuring high traffic websites can handle the load and providing a failover if a server becomes unresponsive.

When you request a website with a load balancer, the load balancer will receive your request first and then forward it to one of the multiple servers behind it. The load balancer uses different algorithms to help it decide which server is best to deal with the request. A couple of examples of these algorithms are round-robin, which sends it to each server in turn, or weighted, which checks how many requests a server is currently dealing with and sends it to the least busy server.



Load balancers also perform periodic checks with each server to ensure they are running correctly; this is called a health check. If a server doesn't respond appropriately or doesn't respond, the load balancer will stop sending traffic until it responds appropriately again.



2\. CDN (Content Delivery Networks) :-

&#x20;  --------------------------------

A CDN can be an excellent resource for cutting down traffic to a busy website. It allows you to host static files from your website, such as JavaScript, CSS, Images, Videos, and host them across thousands of servers all over the world. When a user requests one of the hosted files, the CDN works out where the nearest server is physically located and sends the request there instead of potentially the other side of the world.



3\. Databases :-

&#x20;  ---------

Often websites will need a way of storing information for their users. Webservers can communicate with databases to store and recall data from them. Databases can range from just a simple plain text file up to complex clusters of multiple servers providing speed and resilience. You'll come across some common databases: MySQL, MSSQL, MongoDB, Postgres, and more; each has its specific features.



4\. WAF (Web Application Firewall) :-

&#x20;  ------------------------------

A WAF sits between your web request and the web server; its primary purpose is to protect the webserver from hacking or denial of service attacks. It analyses the web requests for common attack techniques, whether the request is from a real browser rather than a bot. It also checks if an excessive amount of web requests are being sent by utilising something called rate limiting, which will only allow a certain amount of requests from an IP per second. If a request is deemed a potential attack, it will be dropped and never sent to the webserver.



Answer the questions below:

What can be used to host static files and speed up a clients visit to a website?



Answer : CDN

\------



What does a load balancer perform to make sure a host is still alive?



Answer : health check

\------



What can be used to help against the hacking of a website?



Answer : WAF

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

How Web Servers Work :-

\---------------------



1. What is a Web Server?



Answer : A web server is a software that listens for incoming connections and then utilises the HTTP protocol to deliver web content to its clients. The most common web server software you'll come across is Apache, Nginx, IIS and NodeJS. A Web server delivers files from what's called its root directory, which is defined in the software settings. For example, Nginx and Apache share the same default location of /var/www/html in Linux operating systems, and IIS uses C:\\inetpub\\wwwroot for the Windows operating systems. So, for example, if you requested the file http://www.example.com/picture.jpg(opens in new tab), it would send the file /var/www/html/picture.jpg from its local hard drive.



2\. Virtual Hosts :-

&#x20;  -------------

Web servers can host multiple websites with different domain names; to achieve this, they use virtual hosts. The web server software checks the hostname being requested from the HTTP headers and matches that against its virtual hosts (virtual hosts are just text-based configuration files). If it finds a match, the correct website will be provided. If no match is found, the default website will be provided instead.



Virtual Hosts can have their root directory mapped to different locations on the hard drive. For example, one.com(opens in new tab) being mapped to /var/www/website\_one, and two.com(opens in new tab) being mapped to /var/www/website\_two



There's no limit to the number of different websites you can host on a web server.





3\. Static Vs Dynamic Content :-

&#x20;  -------------------------

Static content, as the name suggests, is content that never changes. Common examples of this are pictures, javascript, CSS, etc., but can also include HTML that never changes. Furthermore, these are files that are directly served from the webserver with no changes made to them.



Dynamic content, on the other hand, is content that could change with different requests. Take, for example, a blog. On the homepage of the blog, it will show you the latest entries. If a new entry is created, the home page is then updated with the latest entry, or a second example might be a search page on a blog. Depending on what word you search, different results will be displayed.



These changes to what you end up seeing are done in what is called the Backend with the use of programming and scripting languages. It's called the Backend because what is being done is all done behind the scenes. You can't view the websites' HTML source and see what's happening in the Backend, while the HTML is the result of the processing from the Backend. Everything you see in your browser is called the Frontend.





4\. Scripting and Backend Languages :-

&#x20;  --------------------------------

There's not much of a limit to what a backend language can achieve, and these are what make a website interactive to the user. Some examples of these languages (in no particular order :p) are PHP, Python, Ruby, NodeJS, Perl and many more. These languages can interact with databases, call external services, process data from the user, and so much more. A very basic PHP example of this would be if you requested the website http://example.com/index.php?name=adam(opens in new tab)



(opens in new tab) :-

\-------------------

If index.php was built like this:



<html><body>Hello <?php echo $\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\_GET\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\\["name"]; ?></body></html>



It would output the following to the client:



<html><body>Hello adam</body></html>



You'll notice that the client doesn't see any PHP code because it's on the Backend. This interactivity opens up a lot more security issues for web applications that haven't been created securely, as you learn in further modules.





Answer the questions below:

1. What does web server software use to host multiple sites?



Answer : Virtual Hosts

\------



2\. What is the name for the type of content that can change?



Answer : Dynamic

\------



3\. Does the client see the backend code? Yay/Nay



Answer : Nay

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Quiz :-

\----

Click the "View Site" button on the right. Using everything you've learnt from the other modules, drag and drop the tiles into the correct order of how a request to a website works to reveal the flag.



Note: When placing a tile in the correct position, it will highlight in green. When a tile is in the wrong spot, it will highlight in red. Make sure not to refresh the page, as it will reset the tiles all to blank again!



Lab :-

\----



Step-1 :-

\------

So here we see the correct order of a request to a website works -----



1. Request tryhackme.com in our browser
2. Check Local cache for IP Address
3. Check your recursive DNS server for Address
4. Query root server to find Authoritative DNS server
5. Authoritative DNS server advises the IP address for the website
6. Request passes through a web application firewall
7. Request passes through a Load Balancer
8. Connect to Webserver on port 80 or 443
9. Web server receives the GET request
10. Web Application talks to Database
11. Our Browser renders the HTML into a viewable website



Step-2 :-

\------

After that the popup appear in our web browser and show the flag THM{YOU\_GOT\_THE\_ORDER} and it is our 1st question answer and that's how our 1st question is solved.



Answer the questions below:

1. Flag



Answer : THM{YOU\_GOT\_THE\_ORDER}

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

The CIA Triad Room :-

\-------------------

Task 1 :-

\------

Introduction :-

\-------------

Now that we have gained the mandatory knowledge of the digital world, including the fundamentals of computers, operating systems, software, networks, and the web in the previous rooms, let's start our journey into cyber security and learn how to protect this digital world.



We often hear that cyber security protects the systems, networks, and applications from attacks. But have you ever wondered what cyber security protects inside the digital world? Cyber security focuses on protecting three key aspects, which we will learn in this room. At the end of the room, we will also get a hands-on exercise to validate our knowledge.



Learning Objectives :-

\-------------------

By the end of this room, we will be able to:



Understand the pillars of cyber security

Understand the purpose of Confidentiality, Integrity, and Availability

Recognize Confidentiality, Integrity, and Availability in simple scenarios

Make decisions to preserve these core aspects of cyber security

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

Understanding the CIA Triad :-

\---------------------------

In the past, most information was stored on physical papers. Today, the same information is stored as digital data on systems and communicated over the networks. Without having proper security in place, this digital data can suffer serious consequences. It can be exposed to the wrong people, modified without permission, or unavailable when needed most. So, protecting this digital data has become a core requirement for government, organizations, and individuals.



Image of data transferred from one place to another and modified during the transfer.



However, security does not simply mean stopping attacks or having security tools in place. In cyber security, being secure means ensuring specific conditions for the digital data. These conditions are the key aspects around which the security revolves.



* Confidentiality
* Integrity
* Availability
* 

Together, these three principles explain what cyber security actually protects. These principles are known as the CIA Triad. Pretty much everything you would encounter during your journey through cyber security would revolve around them. You would either defend or attack the digital data to ensure these pillars remain intact.



Confidentiality ensures that sensitive data can only be accessed by authorized individuals. If confidentiality is not maintained, unauthorized individuals can access the data, resulting in financial loss, privacy violations, or legal consequences.



Imagine you are having a private discussion with a friend about a personal matter, and an unknown person deliberately listens in and later uses that information to manipulate you. In this situation, the information you wanted to keep private was accessed by somebody who had no right to hear it. This directly harms confidentiality. In such cases, to ensure confidentiality in the future, you may decide to have such conversations in a secure area and be aware of your surroundings.



Now, let's take an example of the digital world. Imagine you are in a coffee shop and you log in to your social media account using the shop's publicly available network. After a few minutes, you are suddenly logged out, and you can no longer access your account because somebody intercepted your credentials from within the network while you were logging in. This is another example of confidentiality being harmed. To ensure confidentiality in the digital world, processes such as encryption and access controls are employed. These terms might be unfamiliar to you now, which is completely fine since you will be learning all this stuff in your cyber security journey.



The table below lists some examples of situations and whether confidentiality is achieved:



|Situation|Confidentiality Achieved?|
|-|-|
|Your Gmail credentials are written on sticky notes on your office table|No|
|Internal documents of the company are available to the employees who need them for their work|<br />Yes|
|One of your personal documents is available on the internet|No|



Integrity :-

\---------

Integrity ensures that unauthorized individuals do not modify data. Without integrity, data can be altered and no longer be trusted. Unauthorized changes in data can sometimes lead to dangerous consequences.



Imagine your teacher gives you a good grade on your exam, and later somebody modifies that grade before it is submitted to the examination authority. This breaches the integrity of your exam grading. To ensure integrity in the future, your teacher might start noting the grades on a separate sheet and verifying them before final submission to the examination authority.



Now, let's consider a digital world example. Suppose you initiate a bank transfer to an account using your mobile device. Before the transaction completes, someone intercepts it and modifies the receiving account information. This results in the amount getting transferred where it wasn't supposed to. This also breaches the integrity. Several techniques are used to ensure integrity in the digital world, which you will learn during your cyber security journey.



The table below lists some examples of situations and whether integrity is achieved:



|Situation|Integrity Achieved?|
|-|-|
|Data changed through authorised approval|Yes|
|The attendance records of students changed after being locked by the teacher|<br />No|
|Order price modified before checkout|<br />No|



Availability :-

\------------

Availability ensures that data and services are available to authorized users when needed. Although it comes as the third and last pillar of the CIA Triad, it is no less important than the other two. Most businesses rely heavily on their digital services, and if those services become unavailable, there is no more business, causing a huge loss to them. Even a short period of downtime can have serious consequences on the businesses and users.



Imagine you deposit your money in a bank that keeps it very secure, but the bank is closed the day you need your money because of a power failure. Now, even though your money is in a secure place, if you, as the owner, cannot access it, it is useless. This is where availability matters. So, to ensure availability in such a case, your bank would likely deploy an alternative power generator to keep services running even if the main power fails.



In the digital world, many cyber attacks affect availability. For example, attackers send a large number of requests to a website that cannot handle them at once, causing it to go down and the business to suffer. No data is leaked or modified, but still the compromise of availability causes a huge loss. In such cases, websites implement measures to manage the traffic load and block requests when a certain threshold is exceeded, ensuring the website's availability.



The table below lists some examples of situations and whether availability is achieved:



|Situation|Availability Achieved?|
|-|-|
|Critical services disrupted by the installation of a software|No|
|Company's website went offline during business hours|No|
|All the systems are accessible to employees during working hours|<br />Yes|



Answer the questions below:

1. Which pillar of the CIA focuses on preventing unauthorized modification of data?



Answer : Integrity

\------



2\. Which pillar of the CIA focuses on preventing unauthorized access to data?



Answer : Confidentiality

\------



3\. Which CIA pillar ensures data is available to users when needed?



Answer : Availability

\------



4\. Which CIA pillar gets impacted if the data becomes untrustworthy?



Answer : Integrity

\------



5\. What is the term used collectively for all these pillars?



Answer : CIA Triad

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

The Security Mindset :-

\--------------------

By now, you have learned about the CIA Triad (Confidentiality, Integrity, and Availability) and how each of its pillars play their role in protecting the digital information. However, CIA is not just a set of definitions, it's a security mindset of cyber security professionals. When a security incident occurs, it is often explained in terms of what was affected. Security professionals generally by asking questions like:



* Was sensitive data exposed to unauthorized individuals?



* Was data being modified without permission?



* Were systems or services unavailable to users when they needed?



Having a clear understanding of each component of the CIA Triad enables one to assess the impact of any incident and decide on an appropriate response.



Hands-on Scenario :-

\------------------

You are attending a cyber security workshop. As part of engagement exercises, they have given you an exercise to assess your foundational cyber security concepts. One part of the exercise is related to the CIA Triad, which you learned.



In this exercise, you are given nine different security incidents. You have to read them carefully and one by one. After that, you have to determine which part of the CIA triad is affected by them. Drag and drop the incidents in the area they affect the most.



Lab :-

\----

Here we set 3 scenario for confidentiality, integrity, availability



1. Confidentiality :-

&#x20;  ----------------

* The employee salary files are publicly accessible to anyone on the Internet
* Sensitive customer data was leaked through an unsecured backup
* An employee shared the login credentials with an unauthorized person



2\. Integrity :-

&#x20;  ----------

* System logs are deleted to hide activity
* A database record was modified without authorization
* A report was altered, changing financial figures



3\. Availability :-

&#x20;  -------------

* The email server was taken offline due to a denial of service attack
* The company website is unavailable during business hours
* Critical system updates were blocked, preventing services from running



Answer the questions below:

1. What is the flag received after solving the exercise?



Answer : THM{CIA\_IS\_ABOUT\_BALANCE}

\------



2\. CIA Triad is not just a set of definitions; it's a mindset. What type of mindset is it?



Answer : Security mindset

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\------

Conclusion :-

\----------

This room marks your first step into cybersecurity. You have learned a very important thing: What exactly do we protect in cyber security?



By understanding the CIA Triad, you have gained the knowledge of a core cyber security mindset, which is the foundation of many cyber security concepts you will encounter as you continue your journey in this field.



Key Terminology :-

\---------------

Let’s recap the core terms you’ve learned. These definitions will help solidify your understanding before moving on to further learning.



* Confidentiality :-

&#x20;  ----------------

Ensuring digital information is not available to unauthorized individuals.



* Integrity :-

&#x20;  ----------

Ensuring digital information is not modified without permission.



* Availability :-

&#x20;  ------------

Ensuring digital information is not unavailable when needed.



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Cryptography Concepts :-

\---------------------

Task 1 :-

\------

Introduction :-

\------------

Opening question: When you see the little padlock icon in your browser's address bar, what's actually stopping someone from reading or modifying your data as it travels across the internet?

Side-by-side comparison of plaintext and ciphertext communication.



* Why Cryptography Matters

Remember the CIA Triad from the last room? Confidentiality, integrity, and availability are the three pillars of cyber security. We saw how attackers try to break these through disclosure, alteration, and destruction.



Now here's the practical question: how do we actually protect secrets and detect tampering in the real world? That's where cryptography comes in.



A Real-World Scenario :-

\----------------------

Imagine you're running a small medical clinic. You need to send patient records, including names, medical conditions, and treatment history, to specialists and insurance companies over the internet. The problem? Data doesn't travel directly from you to the recipient. It bounces through dozens of computers and routers along the way. Without protection, anyone with access to those systems could read, change, or block your data.

Cryptography solves this by using mathematical rules and secret keys to scramble information into gibberish that only authorised people can unscramble.

In this room, we're keeping things simple. No math background needed. We'll use everyday analogies, plain language, and a hands-on game to show you how cryptography works in practice.



Learning Objectives :-

\-------------------

By the end of this room, you'll be able to:



* Explain what cryptography is and why it matters for protecting confidentiality and integrity.
* Describe the difference between plaintext and ciphertext with actual examples.
* Explain what keys and algorithms are, and why keeping keys secret is critical.
* Explain the difference between symmetric and asymmetric encryption using everyday objects, such as lockboxes and mailboxes.
* Describe how symmetric and asymmetric encryption work together to protect your web browsing.



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

Hiding Information - Symmetric Encryption :-

\------------------------------------------

Opening question: If someone's listening to every single piece of data travelling between two people, how can those two people still share secrets?



Understanding the Basics :-

\------------------------

Before we jump into symmetric encryption, let's define the core terms we'll use throughout this room:



1. Plaintext :-

&#x20;  ----------

A message you can read normally. Like HELLO or Patient name: Alice Smith.



2\. Ciphertext :-

&#x20;  ----------

A scrambled version that's not supposed to make sense. Like KHOOR or Sdwlhqw qdph: Dolfh Vplwk.



3\. Key :-

&#x20; -----

The secret ingredient that controls how scrambling and unscrambling work. Think of it as a password that the algorithm uses.



4\. Algorithm :-

&#x20;  ----------

The public recipe—the set of steps that explain how to use the key on the message. Everyone can know the algorithm. Security comes from keeping the key secret.





Real-world cryptography is way more sophisticated than what we'll use here. But the basic pattern stays the same:



i) Encryption process :-

&#x20;  ------------------

plaintext + encryption algorithm + key  → ciphertext



ii) Block diagram of encryption using a secret key and then



iii) Decryption process :-

&#x20;    ------------------

ciphertext + decryptiong algorithm + key   → plaintext



iv) Block diagram of decryption using a secret key



The Lockbox Analogy :-

\-------------------

Think about a physical lockbox :-

\------------------------------

* The algorithm is how the lock works. Anyone can see you insert a key and turn it, hence it's not secret.
* The key is your specific metal key. Only people with that exact key can open your box.
* The plaintext is the letter inside the box.
* The ciphertext is that locked box travelling through the postal system.



Nobody tries to hide how locks work to make them secure. Security comes from keeping your key private and this same principle applies to cryptography. Algorithms are usually public and tested by experts worldwide. The security comes from keeping keys secret.



To put it more practically, Alice wants to send Bob a secret letter, but it must go through the public postal system, where anyone could open it and read it.



Here's what she does:



* She writes her message (the plaintext) on paper.
* She puts the letter in a sturdy lockbox.
* She locks it with a padlock using her key.
* She sends the locked box (the ciphertext) through the mail.



When Bob gets the box, he uses his copy of the same key to unlock it and read the message. Anyone who intercepts the box along the way sees a locked metal box. Without the key, it's useless. The message stays private.



That's symmetric encryption in a nutshell: one key locks the box, the same key unlocks it.



Illustration of symmetric encryption. Alice and Bob each hold a matching key. Alice sends a locked box labeled "CIPHERTEXT" through a cloud filled with masked attackers. A white arrow shows the box reaching Bob, who can open it with his copy of the same key.



Plaintext versus Ciphertext :-

\---------------------------

* Now, how does this look when dealing with text or data? Say Alice wants to send:



HELLO



That's the plaintext—the readable message.



* Alice uses an algorithm and a secret key to scramble it. After scrambling, it becomes:



KHOOR



That's the ciphertext. To anyone without the key, KHOOR is meaningless. The key point: ciphertext should look like random nonsense to anyone who doesn't have the key.



Bob receives KHOOR, uses the same key and algorithm, and unscrambles it back to HELLO.



The Caesar Cipher :-

\-----------------

Algorithm Plus Key :-

\------------------

To make this concrete, we'll use something called the Caesar cipher. It's straightforward, which makes it perfect for learning (but terrible for real security—more on that in a minute).



The Caesar cipher is named after Julius Caesar, who reportedly used this technique over 2000 years ago to send military messages. Even back then, people understood the value of keeping communications secret.



How It Works :-

\------------



The Caesar cipher shifts each letter in your message by a fixed number of positions in the alphabet. That fixed number is your key.A Caesar cipher wheel showing how letters are shifted by a key of +3. The outer ring lists the plaintext alphabet, and the inner ring shows the corresponding ciphertext letters three positions ahead.



Let's say the key is 3 :-

\----------------------

* A shifts forward 3 spots to become D
* B becomes E
* C becomes F and so on.
* X becomes A (it wraps around to the start)
* Y becomes B
* Z becomes C



If Alice wants to encrypt HELLO with a key of 3:



* H → K
* E → H
* L → O
* L → O
* O → R



So HELLO becomes KHOOR.



To decrypt KHOOR, Bob shifts each letter backwards by 3:



* K → H
* H → E
* O → L
* O → L
* R → O



He gets HELLO again. Magic? Nope. Math.



With the Caesar cipher :-

\----------------------

The algorithm (shift each letter by some number) is completely public. Everyone can know how it works.

The key (the number 3 in our example) is what's secret. Only Alice and Bob know this number.

If someone intercepts KHOOR but doesn't know the key, they'd have to try all 25 possible shifts (1 through 25) to find the right one. For a human, that's tedious; for a computer, that takes about a millisecond.



Here's the thing: The Caesar cipher is not secure and is never used in real systems. It's way too easy to compromise and decrypt messages. We're using it here purely because it's simple to understand and shows you how keys and algorithms work together.



Real algorithms like AES (Advanced Encryption Standard) are vastly more complex and secure. But they follow the same basic idea: algorithm + key + plaintext → ciphertext.



Symmetric Encryption Explained :-

\-------------------------------

The Caesar cipher is an example of symmetric encryption. This means that:



* The same key encrypts (locks) and decrypts (unlocks) the message.
* Both sender and receiver need a copy of that key.
* The key has to stay secret from everyone else.



Some of the benefits of using symmetric encryption are:



* It's fast. Symmetric algorithms can churn through huge amounts of data really quickly.
* It's efficient. Perfect for encrypting files, hard drives, and network traffic where speed matters.



However, there's a catch to this efficiency:



How do Alice and Bob share that key safely in the first place?



If they send the key over the internet in plain view, an eavesdropper can grab it. Then that eavesdropper can decrypt every future message.



You might think, "Just encrypt the key!",  but then you'd need another key to encrypt that key, and then another key for that key, and you see the problem. Infinite regress.



This is called the key distribution problem, and it's the Achilles' heel of symmetric encryption when used alone.



* Plaintext :-

&#x20;  ---------

The original, readable message before encryption.



* Key :-

&#x20;  ----

A secret value that controls how the cipher transforms the message.



* Ciphertext :-

&#x20;  ----------

The encrypted, scrambled message after applying the cipher.



* Caesar Cipher :-

&#x20;  -------------

A substitution cipher that shifts each letter by a fixed number of positions.



* Brute Force :-

&#x20;  -----------

Trying all possible keys until finding the correct one.



We'll solve this in the next task with asymmetric encryption—a clever approach that uses two different keys instead of one.



Try It Yourself: The "Secret Message Rescue" Game.

Time to put this into practice.



In this game, you're helping a security team that's being monitored on their office Wi-Fi. Attackers are watching everything. The team uses a simple Caesar cipher to communicate safely, and you need to:



* Decrypt secret warnings that were intercepted.
* Encrypt new messages before sending them.
* The game uses the Caesar cipher with different shift keys. You'll adjust the key, watch the message change, and submit your answers.



Remember: this is purely educational. Real systems don't use the Caesar cipher because it's laughably weak.



Lab :-

\---

Step-1 :-

\-------

Here first see that our team get the cypher text DWWDFN WRPRUURZ which was sent using a shift key of 3. Use the cipher tool above to decrypt it and submit the original message. It is our shared key which plaintext we get ATTACK TOMORROW by giving the cypher text and choose shift key 3.



Step-2 :-

\-------

Now The team needs to share a temporary password: SECRET. Encrypt it using a shift key of 5 before sending it over the network. So here now we copy this plain text and choose shift 5 and click on encrypt and we get the encrypted cipher XJHWJY which now our team sent over the network.



Step-3 :-

\------

Now This message was encrypted, but the team doesn't know the key used! Try different shift values in the cipher tool until you find one that produces a readable English sentence. and the cyber text we have is ESP DJDEPX TD LE CTDV but we don't know that what shift value is used and we need to decrypt. So now we one by one increase the shift value from 0 and in that increasing process in shift value 11 we see that our cipher text ESP DJDEPX TD LE CTDV is decrypt THE SYSTEM IS AT RISK.



Step-4 :-

\------

An attacker has sent a coded message. The key is unknown, but with only 26 possible shifts, you can try them all! Decrypt this final warning. so we have cypher text XLMW MW XLI JMREP GSHI and we increase the shift value and in shift value 4 we get the plain text of this cipher text and plain text we get is THIS IS THE FINAL CODE.



Step-5 :-

\------

Now we get the flag after solve this 4 scenario which is THM{CAESAR\_CIPHER\_MASTER\_2026}. That's How we solve the first question answer.



Step-6 :-

\------

Now we have the plain text CYBER and here given shift value is 5 now we get the ciphertext HDGJW which is our second question answer.



Step-7 :-

\------

Now we have the cipher text FVZCYR PNRFNE PVCURE and we don't know the shift key value so we simply increase the value and at 13 value we get the plain text SIMPLE CAESAR CIPHER. That's how our final question answer is solve.



Answer the questions below:

1. What's the flag you received after completing all levels of the Secret Message Rescue game?



Answer : THM{CAESAR\_CIPHER\_MASTER\_2026}

\------



2\. Using the Caesar cipher with a key of 5, what does CYBER become when encoded? (Uppercase, no spaces.)



Answer : HDGJW

\------



3\. Using the Caesar cipher, find the correct key and decode the following secret message: FVZCYR PNRFNE PVCURE.



Answer : SIMPLE CAESAR CIPHER

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

Sharing Keys Safely: Asymmetric Encryption :-

\-------------------------------------------

Opening question: If Alice and Bob have never met and can't safely send a key over the internet, how can they start encrypting messages to each other?

The Key Distribution Problem

In the last task, we saw how symmetric encryption works. Alice and Bob use the same key for both encryption and decryption. It's fast and efficient.



However, we also hit a wall: how do they share that key safely in the first place?



If they send it in plaintext, an attacker grabs it. If they encrypt the key, they need another key, which brings us right back to the same problem.



Enter asymmetric encryption.



Two Keys Instead of One :-

\-----------------------

Asymmetric encryption uses two mathematically linked keys:



* A public key that anyone can know and use.
* A private key that only one person keeps secret.



Here's the clever part :-

\----------------------

* If you encrypt something with someone's public key, only their private key can decrypt it.
* If you encrypt something with your private key, anyone with your public key can decrypt it (this is primarily used for digital signatures, which we won't delve into here).



The two keys are connected by some serious maths, but it would take an ordinary computer hundreds or even thousands of years to recover the private key from the public key. This computational difficulty is what makes asymmetric encryption secure.



The Mailbox Analogy :-

\-------------------

Illustration of asymmetric encryption. Alice places an envelope into a public mailbox labeled “Public Key (Anyone can use this).” Bob kneels beside it holding a key labeled “Private Key (Only Bob can open this),” representing the use of different keys for encryption and decryptionLet us use a physical mailbox on a street corner as an example:



* The mail slot at the top is the public key. Anyone walking by can drop off a letter. It's completely open and accessible.
* The locked door at the front is the private key. Only the mailbox owner has the key to open it and grab the letters.



When Alice wants to send Bob a secret :-

\-------------------------------------



* Alice finds Bob's public key (the mail slot). This isn't a secret—Bob can post it on his website or email it around.
* Alice writes her message, encrypts it with Bob's public key, and sends it.
* Only Bob can decrypt it because he is the only one with the private key (the key to the door).
* Even if an attacker intercepts the encrypted message, they can't decrypt it without Bob's private key.



Solving the Key Distribution Problem

With asymmetric encryption, Alice and Bob don't need to share a secret key beforehand. A simple flow of events can be as follows:



* Bob creates a public key and a private key on his computer. He keeps the private key to himself and shares the public key with the world.
* Alice grabs Bob's public key (maybe from his website or a key server).
* Alice encrypts her message using Bob's public key and sends it off.
* Bob receives it and decrypts it using his private key.
* At no point did they need to exchange a key over the network secretly. The only key that travelled publicly was Bob's public key, which isn't secret by design. That's the solution to the key distribution problem.



Alice and Bob using a public and private key pair to exchange messages



Real-world Use: HTTPS :-

\---------------------

The most common everyday use of asymmetric encryption is in HTTPS—the secure protocol you use whenever you see that padlock in your browser.



Here's what happens when you visit https://google.com:



* Your browser requests the website's public key.
* The website sends back its public key wrapped in a certificate (more on this shortly).
* Your browser and the website use asymmetric encryption to agree on a shared secret (a symmetric key) without anyone else being able to see it.
* From there on, they switch to fast symmetric encryption using that shared secret for the rest of the session.



This combo is sometimes called a hybrid approach :-

\------------------------------------------------



* Asymmetric encryption solves the problem of key distribution.
* Symmetric encryption handles the heavy lifting because it's way faster.
* You might wonder: how does Alice know the public key really belongs to Bob, and not to an attacker pretending to be Bob? That's where certificates come in.



A certificate is a digital document that :-

\-----------------------------------------

* Contains someone's public key.
* States who that key belongs to (like example.com).
* A trusted authority digitally signs it, called a Certificate Authority (CA).
* Your browser and operating system come preloaded with a list of trusted CAs. When a website hands over a certificate:



* Your browser checks that a trusted CA signed it.
* Your browser checks that it's still valid (not expired or revoked).
* If everything looks good, your browser shows the padlock and trusts the public key.
* If something's off—perhaps the certificate has expired or was signed by an untrusted authority—your browser displays a warning and may refuse to connect.



Viewing a Certificate In Your Browser :-

\-------------------------------------

You can peek at the certificate for any HTTPS site right now. These steps can guide you to view certificates :-

\-------------------------------------------------------------------------------------------------------------

* Visit any HTTPS site (try https://www.tryhackme.com).
* Click the padlock icon in the address bar.
* Look for something like "Certificate", "Connection is secure", or "View certificate".



A window opens showing details like :-

\-----------------------------------

* Issued to: The website's domain.
* Issued by: The CA that signed it.
* Valid from / Valid until: The certificate's expiration dates.



This is how your browser knows it's talking to the real website and not an attacker's fake version.



Symmetric vs Asymmetric: Side by Side

In summary, let's compare the two approaches we've covered:



|Feature|Symmetric Encryption|Asymmetric Encryption|
|-|-|-|
|Number of keys|One key for both encrypting and decrypting|Two keys: public and private|
|Key sharing|Both people need the same secret key|Public key can be shared openly|
|Speed|Very fast|Slower (used for small amounts of data)|
|Main use|Encrypting bulk data (files, network traffic)|Sharing keys, securely and digital certificates|
|Analogy|One key locks and unlocks a box|A mailbox: anyone posts, only the owner retrieves|



In practice, real systems use both:



* Asymmetric encryption initiates a connection and securely shares a symmetric key.
* Symmetric encryption takes over for the remainder of the session to efficiently handle data.



This is how HTTPS, VPNs, and encrypted messaging apps all operate.



Answer the questions below:

1. In asymmetric encryption, which key stays secret?



Answer : private key

\------



2\. With asymmetric encryption, Alice can encrypt a message using Bob's public key, and only Bob's private key can decrypt it. Yay or Nay?



Answer : Yay

\------



3\. What problem does asymmetric solve that symmetric cannot?



Answer : key distribution

\------



4\. After initial asymmetric exchange in HTTPS, what encryption type handles bulk data?



Answer : symmetric

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Conclusion :-

\----------

What We've Covered

In this room, we explored the basics of cryptography and its role in protecting confidentiality—one of the three pillars of the CIA Triad. We covered the core ideas:



* Plaintext is what you can read. Ciphertext is scrambled gibberish.
* A key is the secret that controls scrambling and unscrambling.
* An algorithm is the public method for using the key.



We looked at two flavours of encryption:



* Symmetric encryption uses a single key for both encryption and decryption. It's fast and efficient, but you need a secure way to share that key. We used the Caesar cipher to see how this works.
* Asymmetric encryption uses two linked keys: a public key that anyone can use and a private key that only one person keeps. This solves the key distribution problem and powers the initial handshake for HTTPS connections.



We also saw how real systems combine both types:



* Asymmetric encryption sets up a shared key at the start.
* Symmetric encryption handles the actual data because it's faster.



That combo is what protects your passwords, banking details, and messages when you see that padlock in your browser.



Cryptography is one of the most critical tools in a defender's arsenal. It protects confidentiality and integrity, and it's the backbone of almost every secure system you use online. But it's not magic. It's one layer in a much bigger security picture that includes:



* Strong password practices.
* Secure key storage.
* User awareness and training.
* Regular software updates.
* Monitoring and incident response.

\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Become a Hacker Room :-

\--------------------

Task 1 :-

\-------

What Is Offensive Security?

Answer : Offensive Security focuses on proactively testing systems by attempting to break into them, with the goal of identifying weaknesses before real attackers can exploit them. If you’ve been working through the Pre Security path, you’ve already built a solid foundation in how computers, networks, and web technologies work. In this room, you’ll take the next step and start applying that knowledge from an attacker’s perspective.



In offensive security, you start with questions: What is exposed? What can be accessed? What assumptions does the system make? A hacker applies these questions methodically, observing how systems respond to unexpected input. In this room, “hacking” refers to penetration testing, an ethical, legal, and structured method for identifying weaknesses so they can be addressed. A hacker is someone who uses these skills positively to improve system security. In the following tasks, you’ll learn common offensive security terminology and methodology, then apply those concepts in a hands-on scenario to see how attackers identify and chain weaknesses together as they move deeper into a target.



Learning Objectives :-

\-------------------

* Explain what offensive security is and understand why it is used to improve system security
* Recognize common terminology and methodology used in offensive security
* Practice ethical hacking techniques in a safe, permission-based environment
* Identify next steps and learning paths to continue your offensive security journey



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\------

Finding Weaknesses :-

\------------------

Before we begin our ethical hacking exercise, it is important to understand some common terminology you'll encounter throughout the room and in your cyber security learning journey. In our exercise, you'll interact with a web application and begin thinking like an attacker, safely and responsibly. This approach is known as offensive security. Rather than waiting for attackers to strike, offensive security professionals proactively test systems to find weaknesses before malicious hackers do.



Core Offensive Security Terms :-

\------------------------------

* Red Teaming :-

&#x20;  -----------

A structured, authorized attack methodology that simulates a real adversary to test the effectiveness of defenses and find vulnerabilities within a defined scope



* Penetration Test :-

&#x20;  -----------------

A structured security assessment where an authorized tester attempts to identify and exploit vulnerabilities within a defined scope to understand real-world risk



* Vulnerability :-

&#x20;  -------------

A weakness or flaw in a system, application, or configuration that an attacker could abuse



* Exploit :-

&#x20;  -------

A technique or method used to take advantage of a vulnerability to achieve a specific outcome, such as accessing restricted functionality or data



* Scope :-

&#x20;  ------

The boundaries of what is allowed to be tested during an engagement. Scope defines which systems, applications, and actions are permitted, and what is off-limits

While some terms are used interchangeably, they all share one critical rule: permission. Ethical hacking, also known as penetration testing, is the practice of testing systems in a controlled and legal manner. Ethical hackers are explicitly allowed to test systems within a defined scope, making this work intentional and safe. In the real world, organizations hire penetration testers or red teams to simulate attacks against their own systems and networks. The purpose isn’t to cause damage; it’s to test the strength of security controls and defenses, uncover gaps, and help teams improve their overall security posture.



Getting Hands-On :-

\----------------

Now that you’re familiar with some common offensive security terminology, it’s time to put those concepts into practice. In this task, you’ll interact with a web application and begin thinking like an attacker, safely and responsibly.



Scenario and Tools :-

\------------------

After months of working on his business idea, Mike is finally ready to launch his website. He has invested a significant amount of time and effort in developing a product that he believes users will love. However, Mike is also aware that businesses of all sizes are targeted by attackers daily. Before going live, he wants reassurance that no sensitive or unintended pages have been left publicly accessible. You’ve been asked to perform an assessment of his web application and identify any exposed areas that could pose a security risk. Your goal is to find these weaknesses before real attackers do, and help Mike launch with confidence. When you’re ready, click the View Site button above to access the web application and begin your assessment.



* In the upper-right half of the split-screen, you can see a simulated browser window displaying the URL http://www.onlineshop.thm/, as shown in the figure below.



* A screenshot of the online shop from the static site practical showing the URL http://www.onlineshop.thm/.



* In the lower right half, you can access a simulated terminal, as seen below, to use the available security tools later in this exercise.





Terminal :-

\--------

Welcome to fish, the friendly interactive shell

user@thm \~>

Beginning Your Assessment



Remember, Mike has asked you to assess his web application and spot any weaknesses. There are several strategies you could use to approach this assessment, but let's begin by identifying any hidden pages that shouldn't be accessible to the public. Let's test out the pages below by adding them at the end of the http://www.onlineshop.thm/ URL in the address bar. Note that upon testing a URL that does not exist, you will see an Error 404 response on the screen, indicating that the requested page cannot be found. See if you can find the hidden page now!



* sitemap Use the browser to check if http://www.onlineshop.thm/sitemap exists
* mail Continue checking for the remaining pages
* register
* login
* admin



A screenshot of the online shop from the static site practical showing the url http://www.onlineshop.thm/ and an arrow with the text “Test Your Pages Here”.



Using Automated Tools :-

\---------------------

That approach worked great, and you should have been able to identify the hidden page successfully. Entering URLs manually is not a big deal if you have a limited number of pages to test, but what if you have a long list of potential pages? One tool in an ethical hacker's arsenal is Gobuster. This tool runs in the terminal and automates the scanning for web pages. Head to the terminal in the bottom half of your split-screen view and enter the following command.



* gobuster dir --url http://www.onlineshop.thm/ -w /usr/share/wordlists/dirbuster/directory-list.txt



Note :-

\-----

To obtain a successful scan result, ensure your input matches the syntax provided above.



The command above is made up of the following parts :-

\---------------------------------------------------



* gobuster The command-line tool used to perform the discovery of web content
* dir Specifies the directory and file enumeration mode, which attempts to discover hidden directories and files on a web server
* \--url http://www.onlineshop.thm/ Sets the target website that Gobuster will scan
* \-w /usr/share/wordlists/dirbuster/directory-list.txt Specifies the wordlist Gobuster will use to guess directory and file names
* A screenshot of the terminal window from the static site practical with an arrow and the text “Enter Your Command Here”.



Lab :-

\---

Step-1 :-

\-------

* First add the webpages name in the url to see what hidden pages can be accessed sitemap Use the browser to check if http://www.onlineshop.thm/sitemap exists
* mail Continue checking for the remaining pages
* register
* login
* admin



http://www.onlineshop.thm/login ---> page open in browser



There we see that we can access the /login page this is manual method and that's how we solve the first question answer.



Step-2 :-

\------

Now we do one more thing that run the automated scanning of hidden directories by using gobuster tool gobuster dir --url http://www.onlineshop.thm/ -w /usr/share/wordlists/dirbuster/directory-list.txt



output :-

\------

user@thm \~> gobuster dir --url http://www.onlineshop.thm/ -w /usr/share/wordlists/dirbuster/directory-list.txt

Gobuster v3.6

\[+] Url: http://www.onlineshop.thm/

\[+] Method: GET

\[+] Wordlist: directory-list.txt

\[+] Negative Status codes: 404

Starting gobuster in directory enumeration mode

/login (Status: 200) \[Size: 314]

Progress: 87664 / 87665 (100.00%)

Finished

user@thm \~>



After the scan done there we see that /login page status code give 200 ok status because it is accessible in a public and reachable so that's how we solve the second number question.



Answer the questions below:

1. Using the manual or automated methods described above, what hidden web page did you discover?



Answer : /login

\------



2\. Based on your Gobuster scan results, what status code is returned when accessing the hidden page?



Answer : 200

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\-------

Exploiting Weaknesses :-

\----------------------

Part of ethical hacking involves learning how to chain weaknesses together. A single weakness may not seem like a critical issue on its own, but when combined with other weaknesses, it can lead to serious consequences. Think of security weaknesses like a line of dominoes. One domino falling on its own doesn’t cause much damage. But when the dominoes are placed close together, knocking over just one can trigger a chain reaction that brings them all down.



In the previous task, discovering a hidden login page was that first domino. On its own, a hidden page might not seem dangerous, but it can become far more serious when combined with other weaknesses, such as weak passwords. Ethical hackers search for and demonstrate these chained weaknesses, showing how minor issues can align to produce a greater impact.



An illustration of a line of dominoes in which half are falling down representing security weaknesses.



Think Like a Hacker :-

\-------------------

To become a hacker, you must think like one. Hackers look beyond whether something works as intended and ask how it might be misused, combined with other behavior, or used for unauthorized access. This means thinking creatively and testing new ideas. Ethical hackers adopt this same mindset, but in a safe and authorized way. They find and prove risks before real attackers can.



Here are some key points to keep in mind as you continue your ethical hacking journey.



* Ask questions: Don't assume a feature works as intended. Instead, ask “What if it doesn't?”
* Test the unexpected: Try actions and inputs that the developers didn't consider
* Chain small weaknesses: A tiny flaw may be harmless alone, but could be connected to create a bigger impact
* Think like an adversary: Think “How would a malicious actor approach this target?”



A Valuable Target :-

\-----------------

Attackers are often interested in gaining valid credentials, such as usernames and passwords, because gaining access can unlock private areas of an application and increase their capabilities. Let’s explore what becomes accessible to an attacker once they gain entry to the private areas of an application.



* Sensitive functionality: Features that perform essential actions, such as modifying data, viewing restricted content, or triggering processes that should only be available to authorized users
* User data: Personal or private information belonging to users, such as names, email addresses, or account details, which attackers may steal, abuse, or sell
* Administrative features: High-privilege functionality that allows attackers to manage users, change settings, or gain full control of the application if accessed
* Further attack opportunities: Authenticated access can expose other vulnerabilities, allowing attackers to expand their access or move deeper into the application

In the previous task, you discovered a hidden page that allows registered users to sign in. While this page may appear harmless, exposing authentication functionality can allow attackers to attempt unauthorized access. In this task, you'll attempt to exploit this weakness by testing whether the login mechanism can be abused.



A screenshot of the /login page from the static site practical.



Getting Hands-On :-

\-----------------

You now know which page you can access, and your next goal is to determine whether you can find a set of working login credentials (username and password) to access the web application. One of the most common usernames is admin so let's begin your attempt here. Like in the previous task, we will begin with a relatively short word list. Go ahead and try the admin username with the list of passwords below.



1. abc123

2\. 123456

3\. password

4\. qwerty

5\. 654321



Were you able to find the password and log in successfully? The username admin paired with one of the passwords above will give you access and present you with your flag.



Hacking Automation :-

\------------------

In the previous task, you learned about and experienced the power of automated tools in ethical hacking. While a short password list may be quick to test manually, real‑world penetration testers often test hundreds or thousands of passwords. In this section, you’ll use Hydra, a password‑testing tool that automates login attempts against a target application using a wordlist. Since we already know the username, Hydra will systematically try each password in the wordlist to see if the login is successful. This technique is known as a dictionary attack, as the tool relies on a predefined list of possible passwords.



Once again, navigate to the terminal in the bottom half of your split-screen view and enter the following command.



* hydra -l admin -P passlist.txt www.onlineshop.thm http-post-form "/login:username=^USER^\&password=^PASS^:F=incorrect" -V



The command above is made up of the following parts :-

\---------------------------------------------------

* hydra The command-line tool used to perform the dictionary attack
* \-l admin Attempts to log in using the username admin
* \-P passlist.txt Specifies the password list to try
* www.onlineshop.thm Sets the target website
* http-post-form Indicates that this is an HTTP POST request form
* "/login:username=^USER^\&password=^PASS^:F=incorrect" Specifies how the login request is sent and how Hydra determines whether a login attempt has failed
* \-V Enables verbose output, which displays each username and password attempted



The command arguments listed above may seem overwhelming at first, but there’s no need to fully understand how they are constructed yet. For now, simply run the command and examine the resulting output to observe how Hydra tests each password in the wordlist to locate valid credentials. The valid password is on the second-to-last line of the results. Much faster than attempting them manually!



Whether you used the manual method of testing each password individually or let an automated tool handle it for you, you should now have the admin password. Congratulations! You’ve completed your first ethical hacking exercise by identifying and exploiting weaknesses within Mike’s web application.



Lab :-

\---

Step-1 :-

\-------

First we give command hydra -l admin -P passlist.txt www.onlineshop.thm http-post-form "/login:username=^USER^\&password=^PASS^:F=incorrect" -V



Output :-

\------



Hydra (https://github.com/vanhauser-thc/thc-hydra) starting

\[WARNING] Restorefile (you have 10 seconds to abort... (use option -I to skip waiting)) from a previous session found, to prevent overwriting, ./hydra.restore

\[DATA] max 16 tasks per 1 server, overall 16 tasks, 14344399 login tries (l:1/p:14344399), \~896525 tries per task

\[DATA] attacking http-post-form://www.onlineshop.thm:80/login:username=^USER^\&password=^PASS^ :F=incorrect

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "123456" - 1 of 14344399 \[child 0] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "12345" - 2 of 14344399 \[child 1] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "123456789" - 3 of 14344399 \[child 2] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "password" - 4 of 14344399 \[child 3] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "iloveyou" - 5 of 14344399 \[child 4] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "princess" - 6 of 14344399 \[child 5] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "1234567" - 7 of 14344399 \[child 6] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "12345678" - 9 of 14344399 \[child 8] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "abc123" - 10 of 14344399 \[child 9] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "babygirl" - 13 of 14344399 \[child 12] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "monkey" - 14 of 14344399 \[child 13] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "lovely" - 15 of 14344399 \[child 14] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "jessica" - 16 of 14344399 \[child 15] (0/0)

\[ATTEMPT] target www.onlineshop.thm - login "admin" - pass "654321" - 17 of 14344399 \[child 6] (0/0)

\[80]\[http-post-form] host: www.onlineshop.thm login: admin password: qwerty

1 of 1 target successfully completed, 1 valid password found

user@thm \~>



Step-2 :-

\-------

Now give the login directory location url in browser http://www.onlineshop.thm/login



Step-3 :-

\------

Now we give there username as admin and password as qwerty because in brute force attack we see that admin user password is qwerty. Now when we click on the Enter button then we see that our secret message is appear which is THM{born\_to\_hack!}. So now that's how we solve the second question answer.



Step-3 :-

\------

So we found the admin password is qwerty so that's is the answer of our 1st question.



Step-4 :-

\------

Now we see in the brute force attack output that total 18 attempt are we do and there we see that 17 password are failed attempt means those 17 passwords are not password of a admin user so that 17 number is our final third number question answer.

&#x20;

Answer the questions below:

1. Using either manual testing or an automated dictionary attack, what password did you discover for the admin user?



Answer : qwerty

\------



2\. After logging in using the password found, what secret message is displayed on the page?



Answer : THM{born\_to\_hack!}

\------



3\. Review the output of your Hydra dictionary attack.

How many failed password attempts were made before the correct password was found?



Answer : 17

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\------

Where to Go From Here :-

\----------------------

In this room, you learned about the role of ethical hackers, became familiar with key terminology and hacking methodologies, and gained hands-on experience using real security tools used by professional red teamers to help secure a web application.



Key Terminology :-

\---------------

* Scope :-

&#x20;  ------

The exact systems and actions allowed during a security test



* Vulnerability :-

&#x20;  -------------

A hidden weakness in a system that an attacker could use to break in



* Exploit :-

&#x20;  -------

A method or technique that takes advantage of a vulnerability



* Enumeration :-

&#x20;  -----------

Collecting details about a system, users, and services to find weak points



* Credentials :-

&#x20;  -----------

Login details such as usernames and passwords that unlock access



* Authentication :-

&#x20;  --------------

The step that checks if someone or something is really who they claim to be when logging in



* Dictionary attack :-

&#x20;  -----------------

Trying a predefined wordlist to guess a password or username



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Become a Defender Room :-

\----------------------

Task 1 :-

\------

What Is Defensive Security?

Answer : Defensive Security focuses on understanding what needs to be protected and implementing security measures to prevent, detect, and mitigate the impact of potential attacks. Defenders work to gain visibility into systems, identify weak points, and ensure that systems remain available and protected, aligning with the goals of confidentiality, integrity, and availability (the CIA triad) you learned about earlier in this module. The goal is to be prepared for incidents and respond when they occur.



In the previous room of this module, Become a Hacker, you explored security from the perspective of an attacker. Ethical hackers use the same techniques as malicious actors to identify weaknesses and help organizations improve their defenses. Defenders, often referred to as the Blue Team, need to understand how attackers think, what they target, and how attacks typically unfold. By identifying critical infrastructure, understanding attackers' goals, and applying defenses, defenders help protect their clients' systems.



Learning Objectives :-

\-------------------

* Understand what defenders protect and why visibility matters
* Identify key parts of a client's environment
* Learn basic methods used to protect common systems and services
* Feel confident starting your defensive security journey



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 2 :-

\-------

Understanding Your Environment :-

\------------------------------

In the previous task, we explored the basics of defensive security. Now, we'll focus on what defenders are responsible for protecting and why understanding the environment matters. Before you can protect anything, you need clear visibility into what exists and how it fits together.  A simple yet powerful way to think about this is to imagine your client's infrastructure as a bustling city. Just like city guards need to know the layout, watch for trouble, and know how to respond, defenders must understand their environment to keep it safe.



An illustration of a city surrounded by a wall that represents the client's infrastructure.



The table below uses a simple city analogy to illustrate how defensive security questions translate into real-world security concepts.



|Defensive Question|City Analogy|Security Equivalent|
|-|-|-|
|What are you protecting? (Systems and Infrastructure)|Homes, buildings, people|Client servers, data, workstations, users|
|Can you see what you are protecting? (Visibility)|Cameras, reports, patrols|Logs, network traffic, alerts|
|What classifies suspicious behavior?|Locked door attempts, circling cars|Repeated logins, unusual IP addresses|
|How do you stop a threat?|Police, blocked roads, curfews|Firewall rules, IP address blocking|



What Can You Do as a Defender?

Once you understand what systems exist and how they can be protected, defenders typically organize their work around a set of foundational security concepts. These concepts apply across nearly all environments and will appear repeatedly as you continue learning defensive security.



* Prevention: Putting security controls in place to stop attacks before they happen, such as firewalls, antivirus software, and regular patching.
* Detection: Monitoring systems and networks to identify suspicious or malicious activity through logs, alerts, and security tools.
* Mitigation: Taking action during an incident to limit damage, such as blocking traffic, isolating affected systems, or disabling compromised accounts.
* Analysis: Investigating what happened, how it happened, and which systems were affected by reviewing logs and other evidence.
* Response and Improvement: Recovering from the incident and improving defenses to reduce the risk of similar attacks in the future.

These concepts form the foundation of defensive security and will help guide your thinking about protecting systems throughout this room and beyond.



What Is Your Scope?

Defenders are not responsible for protecting everything on the internet. They focus on protecting what belongs to their organization or client. This includes the devices people use every day, servers that host applications and data, and the networks that connect systems together. Before any defenses can be applied, defenders must understand what systems exist, what they are used for, and how they fit into the overall environment.



An illustration of binoculars and a computer monitor showing a city outline which represents a defender's scope.



Let's go back to the city analogy we previously used and hone in on aspects of client infrastructure. The list below is not exhaustive, but it will give you a good idea of a sample network you may be tasked with defending in the future.



|System or Infrastructure Component|Purpose|City Analogy|
|-|-|-|
|Employee Devices|Where users work and access company resources|Homes|
|Can you see what you are protecting? (Visibility)|Cameras, reports, patrols|Logs, network traffic, alerts|
|What classifies suspicious behavior?|Locked door attempts, circling cars|Repeated logins, unusual IP addresses|
|How do you stop a threat?|Police, blocked roads, curfews|Firewall rules, IP address blocking|



What Can You Do as a Defender?

Once you understand what systems exist and how they can be protected, defenders typically organize their work around a set of foundational security concepts. These concepts apply across nearly all environments and will appear repeatedly as you continue learning defensive security.



* Prevention: Putting security controls in place to stop attacks before they happen, such as firewalls, antivirus software, and regular patching.
* Detection: Monitoring systems and networks to identify suspicious or malicious activity through logs, alerts, and security tools.
* Mitigation: Taking action during an incident to limit damage, such as blocking traffic, isolating affected systems, or disabling compromised accounts.
* Analysis: Investigating what happened, how it happened, and which systems were affected by reviewing logs and other evidence.
* Response and Improvement: Recovering from the incident and improving defenses to reduce the risk of similar attacks in the future.



These concepts form the foundation of defensive security and will help guide your thinking about protecting systems throughout this room and beyond.



What Is Your Scope?

Defenders are not responsible for protecting everything on the internet. They focus on protecting what belongs to their organization or client. This includes the devices people use every day, servers that host applications and data, and the networks that connect systems together. Before any defenses can be applied, defenders must understand what systems exist, what they are used for, and how they fit into the overall environment.



An illustration of binoculars and a computer monitor showing a city outline which represents a defender's scope.



Let's go back to the city analogy we previously used and hone in on aspects of client infrastructure. The list below is not exhaustive, but it will give you a good idea of a sample network you may be tasked with defending in the future.



|System or Infrastructure Component|Purpose|City Analogy|
|-|-|-|
|Employee Devices|Where users work and access company resources|Homes|
|Web Server|Hosts websites or applications accessed by users|Shop/Public buildings|
|Mail Server|Sends and receives email for the organization|Post office|
|Firewall|Controls what traffic is allowed in or out|City gate|
|Internet|External networks not controlled by the organization|Anything outside of the city|



Answer the questions below:

1. What is the goal when a defender puts security controls in place to stop threats before any damage occurs?



Answer : Prevention

\------



2\. What process involves reviewing logs and evidence to understand how an incident happened and what was impacted?



Answer : Analysis

\------



3\. What flag did you receive after successfully mapping your city infrastructure?



Answer : THM{mapping\_infrastructure!}

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 3 :-

\------

Defending Your Environment :-

\--------------------------

In the previous task, you learned the importance of understanding your environment by mapping your client's infrastructure and gaining visibility into the assets you're responsible for defending. Now, we'll build on that foundation by focusing on how those systems can be protected. As a defender, your role is to understand what exists, consider how it could be abused, and apply protections to reduce risk.



An illustration of a city with a wall surrounding it representing client infrastructure. The city has red lines running through the streets to represent the weaknesses and protections facing the infrastructure.



The Defender Mindset :-

\--------------------

As a defender, your success relies on more than just knowing your environment. You must understand the attackers who want to break into your systems. Instead of viewing your system as separate parts, see them as an interconnected chain. Attackers rarely target a single system. They compromise one asset and pivot to the next, building to their goal.



For example, a malicious email attachment might affect an employee's workstation. From there, an attacker could steal usernames and passwords, access a mail server, and eventually reach sensitive data stored on a database server. Each step builds on the last and is an opportunity for a defender to apply security measures to protect systems.



Key Defender Principles :-

\-----------------------

Threat anticipation: Review the systems you aim to protect and ask, "What if?" Imagine realistic paths an attacker may take to achieve their goal.

Attack awareness: Attacks typically follow recognizable stages. Studying common attack chains and frameworks is incredibly useful for defenders.

Risk prioritization: Not every part of your system carries equal risk. Defenders should identify high-value systems and targets.

Continuous adaptation: Defense is not a one-time set up. Threats and attackers evolve, techniques change, and vulnerabilities emerge.



Available Defenses: Tools to Protect Your City :-

\----------------------------------------------

You previously mapped your client's city to know what's inside. Homes, shops, and public buildings, a post office, a city gate, and everything that lies outside the city walls. Now it's time to explore protection. Defenders use several tools that work together, like having locks on doors, guards at the gate, and alarms inside buildings. No single tool stops every bad guy or malicious attempt, but using a layered set makes it much harder for attackers to succeed. Let's review your client's infrastructure once more and examine potential risks and available protections to ensure their safety.



|System or Infrastructure Component|What Could Go Wrong|Defenses You'll Use|
|-|-|-|
|Employee Devices|Someone clicks a bad link or downloads unsafe software|Antivirus to detect bad programs Regular software updates|
|Web Server|Attackers try to break into the website|Only allow safe traffic Use secure communication|
|Mail Server|Malicious or deceptive emails|Spam filters Scan attachments|
|Firewall|Strangers from the internet try to break in|Firewall rules that control access Block known troublemakers|
|The Outside Internet|External threats come from here|Restrict inbound traffic Monitor for suspicious activity|



Don't worry if some of these defenses feel unfamiliar. As you progress further into defensive security, you'll have many opportunities to explore these tools and protections in detail. This list isn't exhaustive, but it is designed to help you understand how defenders match protections to different systems.



Answer the questions below:

1. Which defender principle focuses on identifying the most critical systems to guide security efforts and focus?



Answer : Risk Prioritization

\------



2\. What flag did you receive after successfully defending your city's infrastructure?



Answer : THM{defensive\_techniques!}

\------



\--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Task 4 :-

\-------

Where to Go From Here :-

\---------------------

Great job, Defender! In this room, you explored the fundamentals of defensive security, learned how to identify and understand client infrastructure, and adopted a defender mindset to anticipate how attacks may occur. By thinking like both an attacker and a defender, you examined how security controls can be applied across multiple layers to reduce risk and protect important systems.



Key Terminology :-

\---------------

* Blue Team: A group of cyber security defenders tasked with protecting systems and responding to threats
* Client Infrastructure: The networks, servers, devices, and applications belonging to an organization that need protection
* Visibility: The ability to see and monitor activity across systems to spot potential issues
* Threat: A potential danger, such as a hacker or malware, that could harm systems or data
* Prevention: Stopping threats before they can cause harm by blocking, restricting, or reducing opportunities for attack
* Detection: The process of identifying threats or suspicious activity in networks and systems
* Mitigation: Actions taken to reduce or stop the impact of a threat once it's identified
* Risk: The likelihood and potential impact of a threat successfully harming an organization



\---------------------------------------------------------------------------------------------END--------------------------------------------------------------------------------------------

