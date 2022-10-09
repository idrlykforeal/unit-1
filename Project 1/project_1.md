# Crypto Wallet

![joker-btc-chaos](https://user-images.githubusercontent.com/100017195/191908697-06100872-4961-4bc8-b5cc-b6800059242e.png)

<sub>Meme from the bitcoin manual</sub>


# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

## Proposed Solution

Design statement:

I will to design and make a digital ledger for a client who is Mr Sato. The digital ledger will be about storing transactions regarding cryptocurrency and is constructed using the software Python It will take until Project Week to make and will be evaluated according to the criterias below.


| Group 1   |              | Group  2  |           |
|-----------|--------------|-----------|-----------|
| Developer | Digital Coin | Developer | Coin      |
| Alex      | Bitcoin      | Alek      | Solana    |
| Bernard   | Ethereum     | Mai       | Dogecoin  |
| Yutaro    | Dogecoin     | Daniela   | BInance   |
| Verlon    | Apecoin      | Kris      | Bitcoin   |
| Oswell    | Tether       | Paula     | Lumens    |
| Thumula   | Tron         | Zaven     | Ethereum  |
| Ainee     | Mana         | Jonathan  | Maker     |
| Lison     | Solana       | Kai       | Avalanche |
| Sabu      | Binance      | Daiichiro | Flow      |
| Emmy      | Polkadot     | Masamu    | Cardano   |
| Maria     | Cardano      | Yasmina   | Zcash     |
| Zelan     | Cosmos       | Jana      | LiteCoin  |
| Manahil   | BinanceUSD   | Lyn       | Iota      |
| Krish     | UsdCoin      | Meisa     | Polkadot  |
|           |              | Mayte     | Cosmos    |
|           |              | Pop       | Ripple    |


### Justify the tools of my solution

I will be using Python for this solution becasue it provides easy data scraping functions and various libraries which could help in providing useful statistic managements to Mr Sato. In addition, python, compared to other older languages, offers programmers the advantage of using fewer lines of code to accomplish tasks, which provides increased simplicity and readability both for programmers and program-readers.

### Justify the structure of my solution

The digital ledger I create is going to be a python project in Pycharm, with a main python file calling different functions pre-written in the library python file and reading, appending, and writing database files. This makes the program more managable as different functions are separately written so the modification of certain files will be more simple. Also, this makes the main python file shorter, which means the structure is going to be more clear and readable.

### Selected cryptocurrency

Bitcoin uses peer-to-peer technology to operate with no central authority or banks; managing transactions and the issuing of bitcoins is carried out collectively by the network. Bitcoin is open-source; its design is public, nobody owns or controls Bitcoin and everyone can take part. Through many of its unique properties, Bitcoin allows exciting uses that could not be covered by any previous payment system.

("Bitcoin", https://bitcoin.org/en/)



## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger is protected by a password.
5. The electronic ledger is able to show total amount of inventories.
6. The electronic ledger is able to show the historical transactions.

# Criteria B: Design

## System Diagram
![IMG_0414](https://user-images.githubusercontent.com/100017195/194740831-d892a600-5650-4218-819d-fd88b317490b.jpg)
*system diagram for the digital ledger*
## Flow Diagrams
<img width="367" alt="register_or_login" src="https://user-images.githubusercontent.com/100017195/194737122-b71c9786-32c1-4428-896e-824f5909b3f8.png">

*flow diagram for register or login function*

<img width="250" alt="register" src="https://user-images.githubusercontent.com/100017195/194737137-79030fe8-989c-4eaa-b12c-64241ba0f352.png">

*flow diagram for register function*

<img width="455" alt="login" src="https://user-images.githubusercontent.com/100017195/194737139-97df1346-c904-43fd-87dd-da32b5a6762f.png">

*flow diagram for login function*

<img width="303" alt="getoptions" src="https://user-images.githubusercontent.com/100017195/194737143-47b303f9-8a1c-4826-bf76-a10816a128fd.png">

*flow diagram for get options function*

<img width="469" alt="transaction" src="https://user-images.githubusercontent.com/100017195/194737145-11a48104-bd63-44a9-939b-cdeaabc828e8.png">

*flow diagram for transaction record function*

<img width="192" alt="history" src="https://user-images.githubusercontent.com/100017195/194741868-cda72f20-09d9-4cbf-8df0-1c65ad051e7e.png">

*flow diagram for printing transaction history*

<img width="276" alt="balance" src="https://user-images.githubusercontent.com/100017195/194741878-a4043a24-e21e-464f-942d-77f884f1fa7d.png">

*flow diagram for printing current balance*

<img width="303" alt="exit" src="https://user-images.githubusercontent.com/100017195/194741893-f8a2cd6a-295b-439c-926f-18f7bb226b72.png">

*flow diagram for exit*

## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create success criteria                                       | To meet with the client and get approval on the criterias                                                       | 10min         | Sep 23                 | A         |

# Criteria C: Development

## Register and login system

My client requires a system to protect the private data. I came up with the solution of using a register and login system that records and verifies the username and password using if conditions and the open command to work with a csv file. Also before loggin in, I also created a function asking the user would like to register first if they haven't done so, or they would like to change the username and password. Here are the 3 functions in Python code:

```.py
def register_or_login()->int:
    '''
    this function returns the option of action from the user whether they would like to register or login with password
    :return: int
    '''
    welcome_msg = "Welcome to your Bitcoin Wallet!".center(len, "=")
    intro='''
    Bitcoin uses peer-to-peer technology to operate with no central authority or banks; 
    managing transactions and the issuing of bitcoins is carried out collectively by the network. 
    Bitcoin is open-source; its design is public, nobody owns or controls Bitcoin and everyone can take part. 
    Through many of its unique properties, Bitcoin allows exciting uses that could not be covered by any previous payment system.
'''
    prompt_msg = "please enter an option [1-2]: "
    content = "OPTIONS"
    menu = '''
    1. Register/Change Password
    2. Login
    '''

    print(cs_yellow, welcome_msg, end_code)
    print(intro)
    print(cs_yellow,content.center(len, "-"), end_code)
    print(menu)
    option = validate_int_input(prompt_msg)
    # validate option
    while option < 1 or option > 2:
        option = validate_int_input(f"{cs_red}invalid option, {prompt_msg}{end_code}")

    return option

def register(uname:str, password:str):
    '''
    This function welcomes the user and saves a user, password in the file user_psw.csv
    :param uname: username
    :param password: password
    :return: nothing
    '''
    file=open("user_psw.csv", "w")
    file.write(f"{uname},{password} \n")
    success_msg="Successfully registered, please move on to log in"
    print(cs_green,success_msg.center(len, "-"), end_code)

def login(username:str, psw:str)->bool:
    '''
    This function verifies the input of the username and password and determines whether login is successful
    :param username: str
    :param psw: str
    :return: bool
    '''
    with open("user_psw.csv", "r") as file:
        info= file.read().strip()
        infos=info.split(",")
        if username==infos[0] and psw==infos[1]:
            return True
        else:
            return False
```

## Getting options from the users
Since this is required by the client that it is a text-based program, getting the option from the user is needed. I decided to write a function that displays and gets the option from the user. Below is the code:

```.py
def get_option():
    '''
    this function returns the option of action from the user
    :return: int
    '''
    loggedin = "You are successfully logged in!".center(len, "-")
    prompt_msg = "please enter an option [1-4]: "
    content = "OPTIONS"
    menu = '''
    1. Withdraw
    2. Deposit
    3. View recent 10 transactions
    4. View your current balance
    '''
    print(cs_green, loggedin.center(len, "-"), end_code)
    print(cs_yellow, content.center(len, "-") ,end_code)
    print(menu)
    option = validate_int_input(prompt_msg)
    # validate option
    while option < 1 or option > 4:
        option = validate_int_input(f"{cs_red}invalid option, {prompt_msg}{end_code}")

    return option
```

## Transaction record

My client requires a system to record details of transactions, so I created a function to append each transactions to database file transactions.csv. Here is the code:

```.py
def transaction(action:str , amount:float, year:int, month:int, day:int , remarks:str):
    '''
    this function helps record the transaction information into the transactions.csv
    :param action: str
    :param amount: float
    :param year: int
    :param month: int
    :param day: int
    :param remarks: str
    :return: nothing
    '''
    file = open("transactions.csv", "a")
    file.write(f"{action},{amount},{year},{month},{day},{remarks} \n")
```

## Print historical transactions

My client requires the ledger to be able to print the details of historical transactions. I created a function that reads from the database file transaction.csv and prints the details of the transaction in a table form. Here is the code:

```.py
def print_transactions():
    '''
    this function reads transactions.csv and prints the transaction history
    :return: none
    '''
    print(cs_blue,"\nTRANSACTION HISTORY".center(106, "*"),end_code,"\n")
    info=[]
    with open("transactions.csv","r") as file:
        raw_transactions=file.readlines()
    for line in raw_transactions:
        line=line.strip()
        values= line.split(",")
        info.append(values)
    print("Action".ljust(15),end=" | ")
    print("Amount".ljust(15), end=" | ")
    print("Year".ljust(15), end=" | ")
    print("Month".ljust(15), end=" | ")
    print("Date".ljust(15), end=" | ")
    print("Remarks".ljust(15), end=" | \n")
    print("".ljust(107 ,"-"))
    for i in info:
        for a in i:
            print(a.ljust(15), end=" | ")
        print()
```

## Print current balance

My client requires to view the current balance. I created a function that reads from the database file transaction.csv and calculates the current balance and displays the current balance. Here's the code:

```.py
def print_balance():
    '''
    this function reads transactions.csv and prints the current balance
    :return:
    '''
    balance=0
    info = []
    with open("transactions.csv", "r") as file:
        raw_transactions = file.readlines()
    for line in raw_transactions:
        line = line.strip()
        values = line.split(",")
        info.append(values)
    for i in info:
        if i[0]=="Withdraw":
            balance-=int(i[1])
        if i[0]=="Deposit":
            balance+=int(i[1])
    print(cs_blue,f"\nYour current balance is {balance}",end_code)
```

## Exit
I created an option for users to exit the program. The exit function also prints a exit message to the user saying goodbye. Here's the code:

```.py
def exit():
    message='''Thank you for using the digital bitcoin ledger, see you next time!'''
    print(cs_blue, message.center(len,"-"), end_code)
```

