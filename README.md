# BrainCracker
A brute forcer for insecure mnemonic BTC brainwallets.

# Concept
Brainwallets are a kind of cryptocurrency wallet where a passphrase that can be used to make addresses is memorized. The idea behind BrainCracker is that since these passphrases are likely made to be easily memorable, they are also likely a lot easier to guess by brute force. Most wallet crackers I've come across attempt to brute force *every* single kind of wallet address. You know... all 2^160 of them. So to avoid making a program that basically explores the Bitcoin equivalent of the Library of Babel, I decided it would be much more practical to try and brute force low entropy brain wallets.

I also intend for this program to be a free, open-source competitor for those "wallet miners" people on Youtube scam you into buying through a Discord server. If people want to spend their money and time on programs with colorful UI's that may or may not work, I'd rather they only spend their money on electricity bills rather than throwing their digi-doubloons into a metaphorical firepit.

# How It Works
BrainCracker is a dictionary attacker program. Using a pre-installed wordlist/dictionary (or one you put in yourself), it progressively goes through all the words on the list or the combinations thereof (such as Bip39 seed phrases). When a word/combination is generated, it will be used to create a private key and then a public key. To make sure BrainCracker doesn't eat up your internet bandwidth, the public key is compared in an offline database of public keys with balances. If the generated public key matches to one in the database, it will be saved in hits.txt.

# Project Ideas/Goals
1. Built-in Bip39 and CrackStation dictionary.
2. Create cool-looking GUI (maybe similar to Bitcoin Core GUI's aesthetic) to automate typing terminal commands.

# Credits
This project will likely be based on https://github.com/adrijano/Bitcoin-wallet-cracker or https://github.com/Isaacdelly/Plutus.

# Donate
Programming something like this is kinda hard, so I'd appreciate if you could send me a few digital doubloons for my trouble.

BTC: bc1qysfa36tfz33xytslluj3hjppm5g4zyn0dmv37r

XMR: 88MHsEonZBTChA6hQUXm9gRaiVUh2tGm63DBniQSaJjMCUMsb7Lt2WCYExB55znKAPRm8aU3MC1vNFWBuVc6CvmxGshdhgV
