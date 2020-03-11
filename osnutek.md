V sklopu tega projekta bomo v ekipi analizirali podatke angleške prve nogometne lige skozi zadnjih 10 let. Osredotočili se bomo na nedavne sezone (18-19, 17-18) v katerih bomo analizirali podatke vseh tekem. <br>
Cilji: <br>
    1. Analiza učinkovitosti ekip v sezoni 18/19 v primerjavi z 17/18, ter spremembe v stilu igranja.
       a. Primerjava sprememb na lestvici skozi sezono v primerjav prejšnjo sezono.
       b. Primerjava posesti ter storjenih prekšrkov proti prejšnji sezoni (sprememba v povprečjih)
       c. Primerjava prejetih ter doseženi zadetkov 
       d. Razlika v rezultatih ekipe v prvem ter drugem polčasu, primerjava točk ob polčasu ter ob koncu igre na koncu sezone
    2. Analiza kakovosti sodnikov
       a. Število iger na sodnika in število piskanih prekrškov/prepovedanih položajev na sodnika
       b. Preiskovanje v statistike sodniških odločitev proti določenim ekipam ali najbolj agresivnim ekipam (največ prekrškov) proti               ostalim
       c. Primerjava sodniške zahtevnosti v sojenju zahtevnih tekem (top 6, derbi tekme), iskanje povezanosti med starostjo/krajom                 rojstva z kvaliteto ter priznanostjo sodnika
    3. Statistika uspehov/neuspehov ter presenečenj
       a. Iskanje največjih nogometnih dominanc npr. niz zaporednih zmaganih tekem, največje zmage na posamezni tekmi, forme ekip skozi             sezono
       b. Največji nogometni preobrati skozi sezono npr. vrnitev iz velikega zaostanka na posamezni tekmi, najboljša uvrstitev ekipe, ki           je napredovala iz druge lige ter njihova durabilnost v ligi 
       c. Prikaz rekordov skozi sezone npr. skupne točke ob koncu sezone, najmanj prejetih, največ doseženih zadetkov
    4. Analiza popularnih stavnic skozi sezono
       a. Prikaz največjih presenečenj skozi kvotami na stavnicah
       b. Statistika povprečij kvot za vsako ekipo
       c. Primerjava povprečij kvot ekip skozi leto z dejansko učinkovitostjo ekip
    5. Napoved sezone 19/20
       a. Analiza trendov iz prejšnjih let npr. spremembe v prejetih/doseženih zadetkov, seštevku točk, pozicija na lestvici
       b. Kreiranje in primerjava napovedane lestvice 19/20 sezone s aktualnim razpletom trenutne sezone (29/38 tekem trenutno odigranih) 
   
   
   
   
   
   
Podatke smo pridobili na naslednji spletni strani: https://datahub.io/sports-data/english-premier-league .
Podatki so shranjeni v csv formatu. V eni datoteki se nahaja 380 primerov z 65 atributi (ponekod manjkajo trije atributi stavnic).
Podatkov iz stavnic je preveliko, zato smo si izbrali samo prve 3. B365, BS in BW.
Pomen okrajšav:

Div = League Division
Date = Match Date (dd/mm/yy)
HomeTeam = Home Team
AwayTeam = Away Team
FTHG = Full Time Home Team Goals
FTAG = Full Time Away Team Goals
FTR = Full Time Result (H=Home Win, D=Draw, A=Away Win)
HTHG = Half Time Home Team Goals
HTAG = Half Time Away Team Goals
HTR = Half Time Result (H=Home Win, D=Draw, A=Away Win)

Referee = Match Referee
HS = Home Team Shots
AS = Away Team Shots
HST = Home Team Shots on Target
AST = Away Team Shots on Target
HHW = Home Team Hit Woodwork
AHW = Away Team Hit Woodwork
HC = Home Team Corners
AC = Away Team Corners
HF = Home Team Fouls Committed
AF = Away Team Fouls Committed
HO = Home Team Offsides
AO = Away Team Offsides
HY = Home Team Yellow Cards
AY = Away Team Yellow Cards
HR = Home Team Red Cards
AR = Away Team Red Cards
HBP = Home Team Bookings Points (10 = yellow, 25 = red)  
ABP = Away Team Bookings Points (10 = yellow, 25 = red)

B365H = Bet365 home win odds
B365D = Bet365 draw odds
B365A = Bet365 away win odds
BSH = Blue Square home win odds
BSD = Blue Square draw odds
BSA = Blue Square away win odds
BWH = Bet&Win home win odds
BWD = Bet&Win draw odds
BWA = Bet&Win away win odds
