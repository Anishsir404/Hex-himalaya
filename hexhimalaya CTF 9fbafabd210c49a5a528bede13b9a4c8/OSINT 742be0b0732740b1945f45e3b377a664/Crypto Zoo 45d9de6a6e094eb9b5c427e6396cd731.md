# Crypto Zoo

![Untitled](Crypto%20Zoo%2045d9de6a6e094eb9b5c427e6396cd731/Untitled.png)

This was one of the hardest CTF I tried so many things and finally got it.

Firstly I did research on the attack and find the wallet of a hacker.

[https://etherscan.io/tx/0xaad710b67ffba3e257f74ce70a37732d548549791e963bee137fc2fe49456b0c](https://etherscan.io/tx/0xaad710b67ffba3e257f74ce70a37732d548549791e963bee137fc2fe49456b0c) 

Now, after that, I look at the id with whom there was interaction.

![Untitled](Crypto%20Zoo%2045d9de6a6e094eb9b5c427e6396cd731/Untitled%201.png)

After that, we look into the transaction history of November 26, 2020.

![Untitled](Crypto%20Zoo%2045d9de6a6e094eb9b5c427e6396cd731/Untitled%202.png)

![Untitled](Crypto%20Zoo%2045d9de6a6e094eb9b5c427e6396cd731/Untitled%203.png)

[https://etherscan.io/txs?a=0x973e52691176d36453868d9d86572788d27041a9&p=189](https://etherscan.io/txs?a=0x973e52691176d36453868d9d86572788d27041a9&p=189)

And finally, we found the transaction hash.

![Untitled](Crypto%20Zoo%2045d9de6a6e094eb9b5c427e6396cd731/Untitled%204.png)

[https://etherscan.io/tx/0xfdef5b6f6dece6b29695b9fd8d0cadaff944876e598fd443125e1f8c2db15160](https://etherscan.io/tx/0xfdef5b6f6dece6b29695b9fd8d0cadaff944876e598fd443125e1f8c2db15160)

```powershell
CTF{0xfdef5b6f6dece6b29695b9fd8d0cadaff944876e598fd443125e1f8c2db15160}
```