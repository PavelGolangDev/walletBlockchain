��������� �������� �� ����� Go, � ����� ���������� Visual Studio Code. 
��� ���� ��� �� �� ���������, ��������� ������������� Go.
��������� ����������� ������� ��������� ������ � ������� ��������������. ���� Go ������ � ��������� ���������� PATH,�� ��������� �������� ��������� "go build GOLANG.go".
���� � ���������� PATH ������ �� ���������, ����� C:\(������������ go)\go.exe run C:\(������������ �����)\GOLANG.go

� ��������� ���������� �������� � �������������� ���� ������ BoltDB. ������ ������ ����� ��������� � �����, � ����� ��������
��������� �������� �����������. �������� ��������� �� ������ ���������: 1) ����������� ���� ���� ������ 2) �������� ������� � ��� ���������
3) ���� �������� ��� ������������: - ��������� ����� ��������� - tip ��������������� �� ��� ���������� ������������ � �� �����.
4) ���� ��������� � ����� ���: - ��������� ������� ���� � ����������� � ���� ������ - ��� ����������� ����� ����������� ��� ��� ���������� �����.
� ��������� ��� �� ���������� ��������� �������� ������.
� ������� ����������� ���������� � ������� �� �������. ������� �� ������� ��������������� ����������.
�� ������� ����� �������� ������� 10 BTC. ����������� ������� createblockchain -address "������". ������� ������� ���� 
� ������� �The Times 03/Jan/2009 Chancellor on brink of second bailout for banks�. 
��������� ��������, ������� ����� ��������� � ����� wallet.dat. ��������� � ��������� ����������� � ������� ����������� �������.
������ ���������� �� ����� ���� ����������� ��� ������� ����������� ������.
������� getbalance -address "��������" ������� ������ �� ������.
������� send -from "������" -to "������" -amount "���-�� BTC". ������� ����, � ����������� ��������.
������� printchain ������� ��� ����� � ���������� ��� ���.
������� createwallet ������� ������ � ������� ��� ����� �� �����.
������� listaddresses ���������� ������ ���� ���������� ���������.


����� ���� �������� �� ������������ ��������.


Programm developed by Go language, in the development environment Visual Studio Code.

In programm realize blockchain using a database BoltDB. Data store in file and aft�r closing progress saved.
Blockchain created by algorithm: 1) Open database file 2) Check for blockhain 3) If blockchain present - create
new instance and flag "tip" set in hash last save in database block. 4) If there is no blockchain in the file -
create genesis block and save in database - genesis block hash save as hash last saved block in database.
In the program is implemented CLI interface.
The project also implemented transactions and awards for mining. The reward is set by a constant.
For mining genesis block - reward 10 BTC.
Added wallets that be stored in the wallet.dat file. Acces to wallets is implemented using special addresses.
Now a transaction cannot be made without virtual subscription.
Implemented command (createblockhain -address ""). Create a genesis block.
Command (getbalance -address "address"). Shows the balanc�.
Command (send -from "address" -to "adress" -amount "amount BTC") - creat transfer transaction block.
Command (printchain) displays all blocks.
Command (createwallet) creates a wallet and shows its address.
Command (listaddresses) displays the adresses for all saved wallets.
Part of the code is cut for commercial reasons.


	Legal (Copyright) 2018-2019 @PavelGolangDev
	All Rights Reserved
