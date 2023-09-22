# HelicopterrHelicopterr

![Untitled](HelicopterrHelicopterr%20f0ad2961700c4a37b69d18f143bc940c/Untitled.png)

There were some encoded data in the Challenge and a image of the Helicopter.

On decoding the given data I got the following result.

![Untitled](HelicopterrHelicopterr%20f0ad2961700c4a37b69d18f143bc940c/Untitled%201.png)

Decoded result

```
One of our crucial local transportation vehicle was stolen! Help us find the current owner/owners of the helicopter to get to the theif.
(If there are two owners then combine their names to get the flag
 Eg. for Riya Manoj and Stan Philip the flag is Riya_Stan)
```

Acc. to the decoded value, we had to find the two owners of the manufacturing company of the Helicopter provided in the image.

![Untitled](HelicopterrHelicopterr%20f0ad2961700c4a37b69d18f143bc940c/Untitled%202.png)

Checking the Manufacturing company of the given Helicopter “N505AJ”, I found the company named “JET RANGER X LLC”.

![Untitled](HelicopterrHelicopterr%20f0ad2961700c4a37b69d18f143bc940c/Untitled%203.png)

Checking the Owners of this company I found two names “John” and “Regan” from the site → [https://opencorporates.com/companies/us_ak/10019092](https://opencorporates.com/companies/us_ak/10019092)

![Untitled](HelicopterrHelicopterr%20f0ad2961700c4a37b69d18f143bc940c/Untitled%204.png)

Therefore, according to the decoded text from above I had to add the Owner’s first name with “_” in between them and it was correct.

Flag → CTF{JOHN_REGAN}