SUMMARY :
          Here we are into wallet creation and handling in Algorand SDK . These modules explains and executes the code in a sequencial manner which is given below .
    
PACKAGES USED :
    Importing modules like encoding , kmd ,account , mnemonic from algosdk package .
    
    from algosdk import encoding
    from algosdk import kmd
    from algosdk import account
    from algosdk import mnemonic
    
Special keys:

    kcl = kmd.KMDClient(tokens.kmd_token, tokens.kmd_address)
   i) Here kmd(Key Management Daemon) is primarily responsible for key management and signing the transactions . One of the feature of kmd is it is platform independent that is it can run in any machine for maximum security .
   
ii) It provides a better API(Application Programming Interface) which is used to create new keys,updating and signing new transactions .

   Important steps :
1) Importing kmd module for signing and updating new transactions .
2) Checks if there is an existing wallets and accounts . If there , then retrieving and accessing the all insights of that wallet .
3) If not , create a new wallet that gets the Wallet name , new wallet password as user-input and accessed using loop conditions .
4) Account is generated with kmd and get the mnemonic for address .
5) Now create and sign transaction with kmd . Get the private key for the existing account .
6) Finally wallet is ready !!!!
7) Now send a trasaction to receiver and check whether the transaction is successfully completed .
