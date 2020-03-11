V sklopu tega projekta bomo v ekipi analizirali podatke angleške prve nogometne lige skozi zadnjih 10 let. Osredotočili se bomo na nedavne sezone (18-19, 17-18) v katerih bomo analizirali podatke vseh tekem. <br>
<b>Splošni cilji: </b><br>
 <b>1. Analiza učinkovitosti ekip v sezoni 18/19 v primerjavi s 17/18, ter spremembe v stilu igranja: </b><br>
       a. Primerjava sprememb na lestvici skozi sezono v primerjavi s prejšnjo sezono. <br>
       b. Primerjava posesti ter storjenih prekšrkov proti prejšnji sezoni (sprememba v povprečjih). <br>
       c. Primerjava prejetih ter doseženi zadetkov. <br>
       d. Razlika v rezultatih ekipe v prvem ter drugem polčasu, primerjava točk ob polčasu ter ob koncu igre na koncu sezone. <br>
 <b>2. Analiza kakovosti sodnikov: </b><br>
       a. Število iger na sodnika in število piskanih prekrškov/prepovedanih položajev na sodnika. <br>
       b. Preiskovanje statistike sodniških odločitev proti določenim ekipam ali najbolj agresivnim ekipam (največ prekrškov) proti               ostalim. <br>
       c. Primerjava sodniške zahtevnosti v sojenju zahtevnih tekem (top 6, derbi tekme), iskanje povezanosti med starostjo/krajom                 rojstva z kvaliteto ter priznanostjo sodnika. <br>
 <b>3. Statistika uspehov/neuspehov ter presenečenj: </b><br>
       a. Iskanje največjih nogometnih dominanc npr. niz zaporednih zmaganih tekem, največje zmage na posamezni tekmi, forme ekip skozi             sezono. <br>
       b. Največji nogometni preobrati skozi sezono npr. vrnitev iz velikega zaostanka na posamezni tekmi <br>
       c. Analiza ekip, ki so napredovale iz druge lige ter njihova durabilnost v ligi <br>
       d. Prikaz rekordov skozi sezone npr. skupne točke ob koncu sezone, najmanj prejetih, največ doseženih zadetkov. <br>
 <b>4. Analiza popularnih stavnic skozi sezono: </b><br>
       a. Prikaz največjih presenečenj skozi kvote na stavnicah. <br>
       b. Statistika povprečij kvot za vsako ekipo. <br>
       c. Primerjava povprečij kvot ekip skozi leto z dejansko učinkovitostjo ekip. <br>
 <b>5. Napoved sezone 19/20: </b><br>
       a. Analiza trendov iz prejšnjih let npr. spremembe v prejetih/doseženih zadetkov, seštevku točk, pozicija na lestvici. <br>
       b. Kreiranje in primerjava napovedane lestvice 19/20 sezone z aktualnim razpletom trenutne sezone (29/38 tekem trenutno odigranih). <br><br>
   
   
   
   
   
<b> Podatki: </b><br>
Podatke smo pridobili na naslednjih spletnih straneh: https://datahub.io/sports-data/english-premier-league, (možna uporaba) https://github.com/footballcsv/england, (možna uporaba) https://www.kaggle.com/thesiff/premierleague1819 .
Podatki so shranjeni v csv formatu. V eni datoteki se nahaja 380 primerov z 65 atributi (ponekod manjkajo trije atributi stavnic).
Podatkov iz stavnic je več kot jih potrebujemo, zato smo si izbrali samo prve 3: <b>B365</b>, <b>BS</b> in <b>BW</b>.<br>
Večina podatkov bomo črpali iz dataseta "english-premier-league" z datahuba:<br>
Pomen okrajšav:

Div = League Division <i>(liga)</i> <br>
Date = Match Date (dd/mm/yy) <i>(datum tekme)</i> <br>
HomeTeam = Home Team <i>(domača ekipa)</i> <br>
AwayTeam = Away Team <i>(gostujoča ekipa)</i> <br>
FTHG = Full Time Home Team Goals <i>(goli domače ekipe čez celotno tekmo)</i> <br>
FTAG = Full Time Away Team Goals <i>(goli gostujoče ekipe čez celotno tekmo)</i> <br>
FTR = Full Time Result (H=Home Win, D=Draw, A=Away Win) <i>(rezultat celotne igre)</i> <br>
HTHG = Half Time Home Team Goals <i>(goli domače ekipe v prvem polčasu)</i> <br>
HTAG = Half Time Away Team Goals <i>(goli gostujoče ekipe v prvem polčasu)</i> <br>
HTR = Half Time Result (H=Home Win, D=Draw, A=Away Win) <i>(rezultat polčasa)</i> <br>

Referee = Match Referee <i>(sodnik tekme)</i> <br>
HS = Home Team Shots <br>
AS = Away Team Shots <br>
HST = Home Team Shots on Target <br>
AST = Away Team Shots on Target <br>
HHW = Home Team Hit Woodwork <br>
AHW = Away Team Hit Woodwork <br>
HC = Home Team Corners <br>
AC = Away Team Corners <br>
HF = Home Team Fouls Committed <br>
AF = Away Team Fouls Committed <br>
HO = Home Team Offsides <br>
AO = Away Team Offsides <br>
HY = Home Team Yellow Cards <br>
AY = Away Team Yellow Cards <br>
HR = Home Team Red Cards <br>
AR = Away Team Red Cards <br>
HBP = Home Team Bookings Points (10 = yellow, 25 = red) <br>
ABP = Away Team Bookings Points (10 = yellow, 25 = red) <br>

B365H = Bet365 home win odds <br>
B365D = Bet365 draw odds <br>
B365A = Bet365 away win odds <br>
BSH = Blue Square home win odds <br>
BSD = Blue Square draw odds <br>
BSA = Blue Square away win odds <br>
BWH = Bet&Win home win odds <br>
BWD = Bet&Win draw odds <br>
BWA = Bet&Win away win odds 
