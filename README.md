# PR20ZJMHZK
## Skupina

 * Žan Jurečič
 * Matic Hrastelj
 * Žan Korošak

## Opis problema
Ukvarjali se bomo z analizo in predstavitvijo podatkov iz angleške Premier lige. 
Naši podatki vsebujejo igrane tekme od leta 2015 do leta 2019 in sicer:
  * Datum
  * Nastopajoče ekipe
  * Glaven sodnik
  * Statistika tekme
  * Podatki o napovedih stavnic 
  * itd.
  
Naši osnovni cilji bodo:
  * Analiza učinkovitosti ekip v sezoni 18/19 v primerjavi s prejšnjimi leti, ter spremembe v stilu igranja
  * Analiza kakovosti sodnikov
  * Statistika uspehov, neuspehov ter presenečenj
  * Analiza popularnih stavnic skozi sezono
  * Napoved sezone 19/20
  * itd.
  
  ### Priprava podatkov
  Posamezne ekipe ter sodnike smo realizirali z objekti. Vsaka posamezna ekipa je torej svoj objekt, ki hrani vse podatke o ekipi. <br>
  Podatke smo shranili v več slovarjev. Imamo 3 glavne slovarje, v katerih so shranjeni vsi klubi z njihovimi objekti, vsi sodniki z objekti ter glavne 3 stavnice. 
  
Najprej smo podatke spravili v spremenljivke.
```python
def read_data(data):
    referee_dict = {}
    teams_dict = {}
    betting_sites = {"365": 0, "IW": 0, "BW": 0}
    
    for row in data:
        div = row["Div"]
        date = row["Date"]
        home_team = row["HomeTeam"]
        away_team = row["AwayTeam"]
        full_time_home_goals = row["FTHG"]
          ..........
        draw_BW = row["BWD"]
        away_BW = row["BWA"]
```
Nato smo pa med branjem posodabljali slovarje z novimi podatki:
```python
        curr_match = Match(date, home_team, away_team, full_time_home_goals, full_time_away_goals, full_time_result,
                           half_time_home_goals, half_time_result, hts, ats,
                           hst, ast, hc, ac, home_fouls, af, home_yellow, away_yellow, home_red, away_red)

        referee_dict[referee].add_all([home_yellow, away_yellow, home_red, away_red], curr_match)
        
        if full_time_result == "H":
            curr_home_team.win += 1
            curr_away_team.loss += 1
            
            betting_sites["365"] += float(home_365) - 1
            betting_sites["IW"] += float(home_IW) - 1
            betting_sites["BW"] += float(home_BW) - 1

            
        curr_home_team.add_all(full_time_home_goals, full_time_away_goals,
                               home_yellow, home_red)
        curr_away_team.add_all(full_time_away_goals, full_time_home_goals,
                               away_yellow, away_red)
```
Za začetek smo za sezono 2018/2019 prikazali razporeditev klubov na lestvici z njihovimi točkami:
```python
  p, t = zip(*sorted([[a,b] for a, b in zip(p, t)], key=lambda item: item[0], reverse=False))
  plt.barh(t, p,color=(0, 0.5, 0, 0.5), edgecolor='blue')
  plt.axvline(x=np.mean(p), label="Povprečno število točk", c='r', linestyle="--")
```
![alt text](./images/slika1.png)

 
 
