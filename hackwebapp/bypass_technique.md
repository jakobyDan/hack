Administrátorské ID jsem identifikoval podle specifické chybové hlášky o omezení přístupu pouze z localhostu (127.0.0.1).  
Aplikace nesprávně brala poslední IP adresu z hlavičky X-Forwarded-For, proto stačilo poslat požadavek s hodnotou `-H 'X-Forwarded-For: 127.0.0.1'`.  
Tím se podařilo zobrazit admin profil a získat vlajku z pole „Interní poznámka“.
