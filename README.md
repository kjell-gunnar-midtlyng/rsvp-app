rsvp-app
==================

Må ha:

- Opprette event med registreringsdato
- Påmelding -> Reserveliste hvis fullt
- Epostutsending ved opprettelse
- Epostutsending ved ledig plass

For å slippe å skrive .gradlew overalt, og heller skrive gw ->
- git clone https://github.com/dougborg/gdub.git
- cd gdub
- ./install


Starte opp lokalt
- gw bootRun -Pprofile=dev
(evt. mot postgresql base: gw bootRun -Pprofile=test) 
- cd frontend && gulp deploywatch


Bygge frontend:
- cd frontend && npm install && gulp deploy



Deploye - 
- Endringer i frontend må bygges først:
  -- cd frontend && npm install && gulp deploy
- git commit ...
- git push
- git push heroku master
- (evt. git push prod master)