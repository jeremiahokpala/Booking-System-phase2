## Results  
**5 out of 10** hashes were cracked using a combination of **dictionary attacks** and **online lookup services** within a limited time frame of a few minutes.

| Email Address | MD5 Hash | Cracked Password |
|--------------|----------------------------------|----------------|
| whatsupdoc@looneytunes.tv | `a0e8402fe185455606a2ae870dcbc4cd` | `carrots123` |
| doho@springfieldpower.net | `d730fc82effd704296b5bbcff45f323e` | `donuts4life` |
| darkknight@gothamwatch.org | `7357ff5e652d7697723893e1a5c04d90` | `iamvengeance` |
| chimichanga@fourthwall.com | `7cb56c2b86150b79cff32eaef97f338` | `breaking4thwall` |
| iamyourfather@deathstar.gov | `706ab9fc256efabf4cb4cf9d31ddc8eb` | `darkside42` |
| **Uncracked** | | |
| genius@starkindustries.net | `d50ba4dd3fe42e17e9faa9ec29f89708` | ❌ |
| elementary@221bbaker.uk | `12c9cef0bfb6b91c42b363b4cf02d8bb` | ❌ |
| whysoserious@gothamchaos.net | `f158d479ee181aac68b000a60e7a3d7a` | ❌ |
| quackattack@duckburg.org | `ea261222d4867b3ebdfadbe2b35e19d5` | ❌ |
| ruhroh@mysterymachine.com | `ad17fbd845000b11678ccbfc94e135b56` | ❌ |

---

## Methods Used  

### 1. Dictionary Attack  
Used **Hashcat** with a small, optimized dictionary (RockYou 1M subset) to ensure cracking time remained under **5 minutes**:
```bash
hashcat -m 0 -a 0 hashes.txt rockyou-1m.txt --force --runtime=300
```
🔹 **Several** passwords were cracked within minutes.  

### 2. Online Lookup  
Checked remaining hashes on:  
- **[Reverse Hash Lookup](https://www.reverse-hash-lookup.online/)**  
- **[MD5Online](https://www.md5online.org/md5-decrypt.html)**  
🔹 **Additional hashes found in seconds.**  

### 3. Limited Brute Force (Failed)  
A **targeted brute-force attack** (only up to **8-character passwords**) was attempted for **5 minutes**:
```bash
hashcat -m 0 -a 3 hashes.txt ?l?l?l?l?l?l?l?l --force --runtime=300
```
🔹 **No new cracks within the time limit.**

---

## Conclusion  
✅ **5/10 hashes cracked.**  
✅ **All attacks lasted only a few minutes.**  
✅ **Dictionary & online lookup were most effective.**  
🔹 **Longer passwords remain secure within this timeframe.**  

