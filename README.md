# mRemoteNG-Decrypt

Python script to decrypt passwords stored by mRemoteNG

## Usage
`python3 mremoteng_decrypt.py -s STRING [-p CUSTOM_PASSWORD]`
OR
`python3 mremoteng_decrypt.py -f FILE [-p CUSTOM_PASSWORD]`


## Todo list:
### Try catch needed
Catch exception to revert to default so this doesn't happen:
```
$ python3 mremoteng_decrypt.py -s "s1L[...]Q=" -p grace
Traceback (most recent call last):
  File "/home/a/mremoteng_decrypt.py", line 49, in <module>
    main()
  File "/home/a/mremoteng_decrypt.py", line 45, in main
    plaintext = cipher.decrypt_and_verify(ciphertext, tag)
  File "/usr/lib/python3/dist-packages/Cryptodome/Cipher/_mode_gcm.py", line 567, in decrypt_and_verify
    self.verify(received_mac_tag)
  File "/usr/lib/python3/dist-packages/Cryptodome/Cipher/_mode_gcm.py", line 508, in verify
    raise ValueError("MAC check failed")
ValueError: MAC check failed

$ python3 mremoteng_decrypt.py -s "s1L[...]Q="
Password: 
```
### Update the instructions 
### Add credit for the OG creator

## Disclaimer for "mRemoteNG-Decrypt":

### Summary:
Exercise responsibility and abide by legal standards while using this software. Unauthorized penetration testing is prohibited and illegal.

### In depth:

- General Use: This software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose, and non-infringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
- Potential Misuse: The software is designed for legitimate purposes only. Any misuse, including but not limited to illegal, unethical, or unauthorized activities, is strictly discouraged and not the intention of the developers.
- User Responsibility: Any person, entity, or organization choosing to use this software bears the full responsibility for its actions while using the software. It is the user's responsibility to ensure that their use of this software complies with local, state, national, and international laws and regulations.
- No Liability: The creators, developers, and distributors of this software are not responsible for any harm or damage caused, directly or indirectly, by the misuse or use of this software.
- Updates and Monitoring: The developers reserve the right to update, modify, or discontinue the software at any time. Users are advised to always use the most recent version of the software. However, even with updates, the developers cannot guarantee that the software is completely secure or free from vulnerabilities.
- Third-Party Software/Links: This software may contain links to third-party sites or utilize third-party software/tools. The developers are not responsible for the content or privacy practices of those sites or software.
- Unauthorized Access: Using "mRemoteNG-Decrypt" to access, probe, or connect to systems, networks, or data without explicit permission from appropriate parties is strictly discouraged, unethical, and illegal. Unauthorized access to systems, networks, or data breaches various local, national, and international laws, and can result in severe legal consequences. Always obtain the necessary permissions before accessing any systems or data. The developers of "mRemoteNG-Decrypt" disavow any actions taken by individuals or entities that use this software for unauthorized activities.

By downloading, installing, or using "mRemoteNG-Decrypt" you acknowledge that you have read, understood, and agreed to abide by this disclaimer. If you do not agree to these terms, do not use the software.
