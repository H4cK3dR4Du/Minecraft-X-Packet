<h1 align="center">✨ 𝕄𝕚𝕟𝕖𝕔𝕣𝕒𝕗𝕥 𝕩 ℙ𝕒𝕔𝕜𝕖𝕥 ✨</h1>

<p align="center">
  <img src="https://img.shields.io/github/license/H4cK3dR4Du/Minecraft-X-Packet.svg?style=for-the-badge&labelColor=black&color=c1121f&logo=IOTA"/>
  <img src="https://img.shields.io/github/stars/H4cK3dR4Du/Minecraft-X-Packet.svg?style=for-the-badge&labelColor=black&color=c1121f&logo=IOTA"/>
  <img src="https://img.shields.io/github/languages/top/H4cK3dR4Du/Minecraft-X-Packet.svg?style=for-the-badge&labelColor=black&color=c1121f&logo=javascript"/>
</p>

<h2 align="center"> 📝 Description 📝 </h2>

<p align="center">
  This repository is used to teach you how to obtain the Minecraft packages (vTable & Signature) using reverse engineering <a href="https://hex-rays.com/ida-free/">(IDA 8.3)</a>.
</p>

<p align="center">
  <b><big>❤️ Made By H4cK3dR4Du ❤️</big></b>
</p>

<h2 align="center"> 🤷‍♂️ Issues / Doubts 🤷‍♂️</h2>

- **If you have any questions do not hesitate to enter my discord: https://discord.gg/raducord**
- **Or if you have any error do not forget to report it in: [issues](https://github.com/H4cK3dR4Du/YOUR-REPO/issues/new)**

<h2 align="center"> 🚀 Get Packet vTable & Signature 🚀 </h2>

### - Requirements And Files:

- **Download IDA 8.3 [here](https://hex-rays.com/ida-free/)**
- **Download Your Minecraft Bedrock Version Database [here](https://www.mediafire.com/folder/ammda8wfvbw9x/The_Flopper_Databases)**
- **Download Cheat Engine [here]([https://git-scm.com/download/win](https://www.cheatengine.org/downloads.php)**

### - Steps To Get Your First Packet vTable & Signature:

*1. Download your Minecraft Bedrock version database from the Flopper databases.*

*2. Download IDA 8.3 and open the Minecraft Windows Client database you downloaded before.*

*3. After opening the database in IDA, you should see the database unpacked.*

*4. You can now view the Minecraft database. Let's start searching for the Packet you want to obtain the vTable and Signature for.*

*5. The first thing we'll do is search for the name of the package you want to obtain. In my case, we'll use MovePlayerPacket. To do that, first click on View > Open Subviews > Strings.*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/ee123350-a9c9-46ae-9a89-bec5af033779)

*6. After that, you should see a menu like this:*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/8b6f0376-c0ec-4de7-bb89-cd294ffc4353)

*7. Now what we'll do is press CTRL+F and search for the Packet name, in this case, MovePlayerPacket*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/298bfc44-1125-4175-b945-d92cd95486ef)

*8. After that, you will see a couple of strings containing the name of your Packet. We need to double-click on the one that solely contains the name of the Packet without any additional information.*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/6444712d-6a47-4889-a077-935e1f9499d1)

*9. Afterwards, you'll see a bunch of data, and the selected line contains the name of your Packet. Next to it, there's a DATA_XREF that we'll need to double-click, which will take us to the location where our Packet is located.*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/39fb0007-8f9a-4858-ac34-5cc2cb06dca7)

*10. After double-clicking the XREF, you'll be taken directly to where the MovePlayerPacket is located. There you can see where the vTable is located; it's always in the .data section above the packet name. Here's how to obtain it:*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/8f815479-eea9-4e30-a43e-499a77d5ab51)

*11. After double-clicking the .data value, you'll be taken directly to the vTable of the packet you searched for earlier. Now, in the following image, I'll show you what the vTable is and how you can obtain the Signature of your Packet.*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/76ff5f53-17d3-495e-9016-5714052ad67a)

*12. Now that you have the vTable, you can also easily obtain the signature. Simply from where you are now, look for the string "off_" above the vTable and press CTRL+X; this will show you the cross-references of the packet. Always select the first one that is selected by default. Here's how to do it:*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/5284dbf8-6c04-453b-bc08-70e39d080c01)

*13. You're on the final step! After clicking on the first automatically selected range, you'll be taken to the origin of the string "off_" you selected earlier. Now, simply select from the line that has been automatically selected to where you see a line with "======" or "-----". Here's how:*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/41fa527d-e391-4cd6-bb83-705775bf9a86)

*14. Finally, just press CTRL+Alt+S to open the SigMakerEx menu (the files you downloaded earlier) and select the 'From address range' option.*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/b1ea6d36-f660-4a13-9333-ab073913b2b0)

*15. Click on 'Continue' and you're done! Now in the console, you have the signature of your Packet. It's automatically copied to your clipboard as well.*

![image](https://github.com/H4cK3dR4Du/Dickeys-Account-Checker/assets/118562174/d799df7d-7087-4e8f-bd13-3bb619f6cebc)

