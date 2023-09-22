# Macro Shot

![Untitled](Macro%20Shot%20bb0f4432ed2a435893a9f7721debff31/Untitled.png)

This was one of my favourite challenges. Firstly, I had no clue what to do but after some research, I found a tool called olevba.

Which gives us the code of macro.

![Untitled](Macro%20Shot%20bb0f4432ed2a435893a9f7721debff31/Untitled%201.png)

So i write a reverse script of it.

```powershell
def reverse_galf(encoded_text):
    original_text = ""
    encoded_numbers = encoded_text.split()
    for num in encoded_numbers:
        ascii_code = int(num)
        char = chr(ascii_code // 10)
        original_text += char
    return original_text

# Example usage:
encoded_output = "670 840 700 1230 1190 1040 1210 950 1000 490 1000 950 490 950 480 1120 510 1100 950 1160 1040 490 1150 950 1090 520 990 1140 480 950 840 870 840 1250"
original_text = reverse_galf(encoded_output)
print(original_text)
```

and boom we got the flag:

```powershell
CTF{why_d1d_1_0p3n_th1s_m4cr0_TWT}
```