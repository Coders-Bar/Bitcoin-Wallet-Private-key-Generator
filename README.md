# Bitcoin-Wallet-Private-key-Generator
This Script is made on Python and its pip Libraries. This Script only works for the bitcoin wallets of Base 58 (P2PKHc), and for cracking the Private key of any Base 58 bitcoin wallet the range of the Private Key must be known to the user by which the time complexity will be less, but even after knowing the range where the targeted private key lies, it will take time as per the start and end range  i.e. 2^0 to 2^256 (Whole Bitcoin key Range), so basically it's a game of luck try it and see if you get lucky and hit the Jackpot!!


This Script is working perfectly as it was made for the sole purpose of cracking the Bitcoin Puzzle "https://bitcointalk.org/index.php?topic=1306983", but unfortunately the range 2^66 is so big to crack by this Script, so sharing this code with everyone maybe someone get lucky and get some BTC...

Procedure to run this Script!...

1. Install Python and open in CMD.
2. Install PIP using this command "python -m pip install pip" in CMD.
3. Now install these modules...
   1. ECDSA
   2. Hashlib
   3. Base58
   4. tqdm
   5. futures
   6. time (if not pre-installed)
   7. math (if not pre-installed)
4. Now go to the directory where the "Hex key finder.py" is saved.
5. run that file in CMD by command "python Hex key finder.py". Before running in CMD please edit the file and input the Base58 wallet address in the file where it says "Input the address here".
6. Now provide the input of the Starting range and Ending Range in the Decimal Format. You can convert the range from this website "https://www.rapidtables.com/convert/number/hex-to-decimal.html"
7. Finally your program will start the sequence from the starting range and if the key is found then the program will save it for you in a text file.

Example:
Lets search for the Private Hex key of the Puzzle no. 15!...
1. Wallet Address: 1QCbW9HWnwQWiQqVo5exhAnmfqKRrCRsvW
2. Range start: 0000000000000000000000000000000000000000000000000000000000004000 (Hexadecimal Number) || 16384 (Decimal Number)
3. Range End: 0000000000000000000000000000000000000000000000000000000000007fff (Hexadecimal Number) || 32767 (Decimal Number)

![Key](https://github.com/Coders-Bar/Bitcoin-Wallet-Private-key-Generator/assets/154334072/fc2ad8dc-184a-45f5-a796-dc90469f0307)

As you can this script divided the whole range into 12 sub-ranges and searched for the key in all the sub-ranges concurrently and it took 0.22445 seconds to search for the key of the above-specified wallet address i.e. puzzle no. 15!!



Good Luck Guyzz!...
