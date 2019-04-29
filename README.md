# No Play No Game


*participant => participant*

*côte => odd*

*pronostiqueur => user*

*tournois => tournament*

*competitions => competition*

*match => match (event)*

*sport => sport*

*pari => bet*


----------------------------------------------------------------------------------
1 user => n tournament
1 user => 1 score
1 user => n bet

1 sport => n competition

1 competition => n match

1 tournament => n competition

1 match => n odd

-----------------------------------------------------------------------------
Database

+ users => id, email, username, password, nbCoins, isActive

+ competitions => id, sportId, name, country, isActive

+ sports => id, name

+ events => id, competitionId, name, startDate, homeTeam, status

+ participants => id, sportId, name

+ odds => id, eventId, type, value

+ bets => id, userId, eventId, tournamentId, nbCoins

+ tournaments => id, createdBy, wonBy, name, startDate, endDate








