
# Wireshark_Packet_Analysis_Toolkit


Introduction
----------------------------------------------------
Welcome back, everyone! I am excited to share this network analysis project using the Wireshark Packet Analysis Toolkit. This project helps showcase practical applications of the Wireshark network protocol analyzer. It involves capturing packets across various protocols (HTTPS, DNS, FTP, etc.) and conducting detailed analyses to identify potential threats and optimize network performance. The repository includes sample .pcap files, comprehensive reports, and a user-friendly guide, making it an excellent resource for network troubleshooting and cybersecurity insights.


Key Takeaways and Instructions 
----------------------------------------------------
[Wireshark for Beginners: Capture Packets]


Task 1:

Install and set up Wireshark on Ubuntu:

[Task 1 Screenshots]

![Topic_1_Screenshot](https://github.com/user-attachments/assets/8007c15b-5b21-4f9e-850b-6e25e2126490)
For these steps, I first downloaded Kali Linux as well as installed Wireshark on Ubuntu Linux. This was executed with the sudo apt install wireshark command.

![Topic_1_Screenshot_2](https://github.com/user-attachments/assets/b311fe13-65e3-4a27-8a9e-3b35aafdb40f)
During this step, I used the sudo usermod -aG wireshark $USER command to create a new user within the Wireshark application. This helps speed up the initialization process.

Task 2:

Start a packet capture on an ethernet port and save it to file:

[Task 2 Screenshots]

![Topic_2_Screenshot_1](https://github.com/user-attachments/assets/3ea952a2-3069-45c5-beeb-722b3a24d744)
During this stage, these were the steps that were used to help save a packet capture within the system. 

![Topic_2_Screenshot_2](https://github.com/user-attachments/assets/80f788e0-373c-4f94-b834-d57f55e8e523)
This was started on the ethernet port (etho) and saved to its .pcap file.

Task 3:

Use a display filter to detect HTTPS packets:

[Task 3 Screenshots]

![Topic_3_Screenshot_1](https://github.com/user-attachments/assets/9e71434e-6d99-4b4a-8de6-5c88f88de60d)
The filter was used to search within the parameters of TCP while looking within port 443 (HTTPS).

Task 4:

Visit a web page and detect its IP address using a display filter:

[Task 4 Screenshots]

<img width="894" alt="Topic_4_Screenshot_1" src="https://github.com/user-attachments/assets/91aca406-2c6d-48b7-9aaa-40f237028f0b" />
This syntax notation of (ip.dst == [source_ip_address]) created a filter regarding an open webpage. Since Firefox was launched, this was the IP address associated with it.

Task 5:
Locate all HTTPS packets from a capture not containing a certain IP address:

[Task 5 Screenshots]

<img width="887" alt="Topic_5_Screenshot_1" src="https://github.com/user-attachments/assets/4568a782-cb1f-4cb6-affb-7aafd57e4def" />
This notation checks the IP address between the listed IP address and the HTTPS port 443 as well within the packet capture.
<img width="943" alt="Topic_5_Screenshot_2" src="https://github.com/user-attachments/assets/64d7968c-14a2-4152-aa9c-aa2d72875f53" />
This notation is used for the parameters between filtering the results of the IP addresses listed excluding the IP address of (172.18.0.27)
<img width="893" alt="Topic_5_Screenshot_3" src="https://github.com/user-attachments/assets/4f38c03c-77bf-4f31-8119-36652eda161a" />
The notation here helps for locating different HTTPS packets that are not within the listed IP address of (172.18.0.27). Additionally, it filters the ports of HTTP and HTTPS as well.


