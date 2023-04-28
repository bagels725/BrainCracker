# BrainCracker
A brute forcer for insecure mnemonic BTC brainwallets.

# Concept
Brainwallets are a kind of cryptocurrency wallet where a passphrase that can be used to make addresses is memorized. The idea behind BrainCracker is that since these passphrases are likely made to be easily memorable, they are also likely a lot easier to guess than, say, secure letter salads like 5KB4cippuEcTAZ6Cc3fqErYtLNKBFeFw6HoTbBdeGouaVShx9ZN.

BrainCracker works by randomly guessing Bip39 seed phrases, generating private and public keys, and comparing them in an offline database to see if they have a balance. If a seed phrase with a balance is found, it's saved to a .txt file.

# Goals
-Allow guessing of both full and partial addresses.
-Create GUI to streamline terminal typing.
