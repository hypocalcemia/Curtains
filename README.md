# Curtains

> [!CAUTION]
> No operating system is 100% secure, and this tool is not magic. Curtains assumes the user is already taking basic security seriously.
> If you are unsure how it works, please read through the code in this repo before using it. You should never run any tool/code you don't understand.


Curtains is a small security hardening tool for Windows. It's purpose is to reduce the impact of common LPE (local privilege escalation) techniques and other security risks.

The primary focus of Curtains is mitigating the Sticky Keys / accessibility executable replacement attack, where an attacker with physical access can replace accessibility tools (such as sethc.exe or utilman.exe) to obtain a SYSTEM command prompt from the Windows login screen. Weird how microsoft never found a way to limit this to only the actual owner/user of windows...

With this project I aim to make these types of modifications easier to detect and harder to abuse on Windows 11 systems.

This project is intended as an additional layer of defense. It does not replace standard security practices such as disk encryption, Secure Boot, and proper physical security.
<br>
> [!IMPORTANT]
> Curtains is **not a replacement for disk encryption**.  
> If someone can boot another OS from an USB Drive, they can still modify the Windows drive offline.
> If you want strong disk encryption, consider **VeraCrypt**.

<hr>



## References

[1] VeraCrypt (open source disk encryption)  
https://github.com/veracrypt/VeraCrypt

