accountstorage klasse:
accountstorage: OK
save: PS
update: første del OK (update account)
andre del OK (delete)
tredje del ser ut til å fungere OK
delete: PS
get: OK
lookup: PS

channelstorage klasse:
channelstorage ok
save PS
update: PS
delete: PS
get: PS
noChangeUpdate: PS
getCurrentVersion: PS
waitNextVersion: OK
givenextversion: OK
lookupChannelForEvent: PS

eventstorage klasse:
eventstorage: OK
save: PS
update: PS
delete: PS
get: PS

SessionStorage klasse:
sessionstorage: OK
save: PS
update: PS
delete: PS
get: PS

UserStorage klasse:
save PS
update PS
delete PS
get PS
lookup PS (denne blir foreløpig ikke brukt?)



To do:
fiks: siden breaker når en bruker prøver å accesse en channel han ikke har tilgang til
fiks: man kan overwrite eksisterende brukere (jeg lagde user14, og logget inn med user14, selv om user14 allerede fantes i databasen)
fiks: setRole-metode i InChat-klassen.
fiks: når setRole-metode er skapt, implementer system i channel som vurderer om bruker kan sende melding osv. hvis banned skal 
      hen helst ikke kunne se channel?






/*
public Stored<User> setRole(Stored<User> user, Stored<Channel> channel, Stored<Permission> permission){
/* Metode som setter de ulike rollene til en bruker.
*  1. Owner: Set role, delete, remove, read and post (any message)
*  2. Moderator: delete, edit, remove, read and post (any message)
*  3. Participant: delete, edit, remove and post (own messages)
*  4. Observer: Read
*  5. Banned: No access to channel
*

        if(permission.equals("owner"){
            true;
        }
        if(permission.equals("banned")) {
            false;
        }
    }
    */