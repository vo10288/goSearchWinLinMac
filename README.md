You must use the correct program for your Operative System, EXAMPLE FOR LINUX :

$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$

./goSearchLinAMD64B -dir /var/log -text "ERROR"


![Schermata del 2025-03-01 16-04-13](https://github.com/user-attachments/assets/7778ae15-bdbf-413c-8760-b99c100283f2)




	       
	
 
 
 
 By Visi@n
	

Uso:
  go run main.go -dir <directory> -type <tipo> [-pattern <regex>] [-text <stringa>] [-csv]

Opzioni:
  -dir <directory>      Directory in cui effettuare la ricerca.
  -type <tipo>          Tipo di ricerca predefinita:
                        - email         → Cerca indirizzi email.
                        - crypto        → Cerca chiavi pubbliche/private di BTC, ETH, Monero, XRP, Solana.
                        - seedphrase    → Cerca mnemonic seed phrase (12, 18, 24 parole BIP39).
                        - iban          → Cerca IBAN bancari.
                        - codicefiscale → Cerca Codici Fiscali italiani.
                        - partitaiva    → Cerca Partite IVA italiane.
  -pattern <regex>      Inserisci un'espressione regolare personalizzata per la ricerca.
  -text <stringa>       Cerca una stringa normale (senza regex).
  -csv                  Salva i risultati in CSV invece di TXT.

Esempi:
  1) Cerca email in una directory:
     go run main.go -dir /home/user/docs -type email

  2) Cerca chiavi crypto e salva in CSV:
     go run main.go -dir /var/logs -type crypto -csv

  3) Cerca con regex personalizzata:
     go run main.go -dir /data -pattern "(error|failed|warning)"

  4) Cerca una stringa normale:
     go run main.go -dir /reports -text "password123"



$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$$
  $./goSearchLinAMD64 -dir /tmp/ -type .csv,.txt,.json,.xml

  
  
  go run main.go -dir <directory> -type <tipo> [-csv]

Opzioni:
  -dir <directory>      Directory in cui effettuare la ricerca
  -type <tipo>          Tipo di ricerca:
                        - email         → Cerca indirizzi email
                        - crypto        → Cerca chiavi pubbliche/private di Bitcoin, Ethereum, Monero, XRP, Solana
                        - seedphrase    → Cerca mnemonic seed phrase (12, 18, 24 parole BIP39)
                        - iban          → Cerca IBAN bancari
                        - codicefiscale → Cerca Codici Fiscali italiani
                        - partitaiva    → Cerca Partite IVA italiane
  -csv                  Salva risultati in CSV invece di TXT

Esempi:
  1) Cerca email in una directory:
     go run main.go -dir /home/user/docs -type email

  2) Cerca chiavi crypto e salva in CSV:
     go run main.go -dir /var/logs -type crypto -csv

  3) Cerca seed phrase BIP39:
     go run main.go -dir /wallets -type seedphrase

