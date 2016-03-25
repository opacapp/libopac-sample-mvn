libopac sample
==============

This is a sample how to use libopac in a maven project

Usage:

    $ mvn package
    $ mvn exec:java -D exec.mainClass=net.opacapp.sample.libopacmvn.HelloOpac

You will receive an output that should look similar to:

    [INFO] Scanning for projects...
    [INFO]
    [INFO] ------------------------------------------------------------------------
    [INFO] Building libopac-sample 1.0-SNAPSHOT
    [INFO] ------------------------------------------------------------------------
    [INFO]
    [INFO] --- exec-maven-plugin:1.4.0:java (default-cli) @ libopac-sample ---
    Hello OPAC!
    Obtaining search fields...
    Found a first search field: Freie Suche
    Searching for 'hello' in this field...
    Found 178 matches.
    First match: SearchResult [id= null, type=SCORE_MUSIC, nr=0, innerhtml=<br />[2015]<br />T 1121 A Songbook<br /><b>Vormerkung (1,- Euro)</b>]
    Fetching details for the first result...
    Got details: DetailledItem [details=[Detail [desc=Titel/Stichwort:, content=25], Detail [desc=Verfasser:, content=Adele], Detail [desc=Hrsg./Bearb.:, content=Norey, Jenni], Detail [desc=Titelzusatz:, content=eleven songs arranged for easy piano], Detail [desc=Ausgabe:, content=Songbook], Detail [desc=Verlag:, content=Wise Publications], Detail [desc=Jahr:, content=[2015]], Detail [desc=Umfang:, content=51 Seiten], Detail [desc=ISBN:, content=1-7855-8222-4], Detail [desc=Preis/Einband:, content=EUR 24,95], Detail [desc=Signatur:, content=T 1121 A], Detail [desc=Notation:, content=T 1121], Detail [desc=Interessenkreis:, content=Songbook], Detail [desc=Inhalt:, content=Enthält: Hello -- Send my Love (To your new Lover) -- I miss You -- When we were young -- Remedy -- Water under the Bridge -- River Lea -- Love in the Dark -- Million Years ago -- All I ask -- Sweetest Devotion]], copies=[de.geeksfactory.opacclient.objects.Copy@296930bd], volumes=[], cover=null, title=25, coverBitmap=null, reservable=true, reservation_info=methodToCall=doVormerkung&katkey=952711969&title=25&author=Adele&context=hitlist, id=952711969, volumesearch=null, mediatype=null]
    [INFO] ------------------------------------------------------------------------
    [INFO] BUILD SUCCESS
    [INFO] ------------------------------------------------------------------------
    [INFO] Total time: 2.760 s
    [INFO] Finished at: 2016-03-25T14:15:26+01:00
    [INFO] Final Memory: 14M/324M
    [INFO] ------------------------------------------------------------------------
