# BrainCracker
A brute forcer for insecure mnemonic BTC brainwallets.

# Concept
Brainwallets are a kind of cryptocurrency wallet where a passphrase that can be used to make addresses is memorized. The idea behind BrainCracker is that since these passphrases are likely made to be easily memorable, they are also likely a lot easier to guess.

BrainCracker is a dictionary attacker program. Using a pre-installed wordlist/dictionary (or one you put in yourself), it progressively goes through all the words on the list or the combinations thereof (such as Bip39 seed phrases). When a word/combination is generated, it will be used to create a private key and then a public key. To make sure BrainCracker doesn't eat up your internet bandwidth, the public key is compared in an offline database. If the generated public key matches to one in the database, it will be saved in hits.txt.

# Project Ideas/Goals
1. Built-in Bip39 dictionary.
2. Allow guessing of both full and partial addresses.
3. Create cool-looking GUI (maybe similar to Bitcoin Core GUI's aesthetic) to automate typing terminal commands.

# Credits
This project will likely be based on https://github.com/adrijano/Bitcoin-wallet-cracker.

# Donate
Programming something like this is kinda hard, so I'd appreciate if you could send me a few digital doubloons for my trouble.

BTC: bc1qysfa36tfz33xytslluj3hjppm5g4zyn0dmv37r

XMR: 88MHsEonZBTChA6hQUXm9gRaiVUh2tGm63DBniQSaJjMCUMsb7Lt2WCYExB55znKAPRm8aU3MC1vNFWBuVc6CvmxGshdhgV
