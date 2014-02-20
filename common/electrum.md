# electrum

> Ergonomic Bitcoin wallet and private key management

- Create a new wallet

`electrum -w new-wallet.dat create`

- Restore an existing wallet from seed offline

`electrum -w recovery-wallet.dat restore -o`

- Create a signed transaction offline

`electrum mktx {{RECIPIENT}} {{AMOUNT}} -f 0.0000001 -F {{FROM}} -o`

- Display all wallet receiving addresses

`electrum listaddresses -a`

- Sign a message

`electrum signmessage {{ADDRESS}} {{MESSAGE}}`

- Verify a message

`electrum verifymessage {{ADDRESS}} {{SIGNATURE}} {{MESSAGE}}`

- Connect only to a specific electrum-server instance

`electrum -p socks5:127.0.0.1:9050 -s 56ckl5obj37gypcu.onion:50001:t -1`