# DWBI-project
Step 1: Data Set Selection
Because we need to create a rich ETL tasks, I took a dataset which contains a large amount of data. And
also, they should contain minimally a year’s data. And I was able to select a tennis log data in which 
contains years thereby I could easily make hierarchies and dimensions etc. And also, I reduce the data 
set columns and rows to create my finalized dataset



Step 2: Preparation of data sources
The tables are in two formats namely CSV and Text
Matches – All details about the Matches (Database table)
Betting-All details about the betting (Text File)
Countries- All details about the players countries(text file)
Players- All details about the players(text file)
Tournaments- All details about the Tournaments(text file)

Step 3 : Solution Architecture
In the ETL process ( Extract, Transform and Load) there are mainly three main components
1. Sourcefile
2. Staging database
3. Data warehous



Step 4 : Data warehouse design and development
For the data warehouse of the tennis data dataset 
,Dimtournament,DimCountrys,DimMatches,DimPlayers,DimFactBettig are implemented as the
dimenshions with DimDate as the date dimension.DimfactBetting is implemented as the fact 
table .DimPlayers is implemented as the slowly changing Dimension.DimPlayers contains a 
foreign key reference to the DimMatches.
