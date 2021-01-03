## Ladda ner och installera verktygen

För att programmera med C# .NET behöver du utvecklingsverktyg och en utvecklingsmiljö. 

Vi börjar med att ladda ner senaste versionen av *utvecklingsverktygen* för .NET. Det kan du göra på den här [sidan](https://dotnet.microsoft.com/download). Hitta knappen på sidan där det står *Download .NET SDK* (alltså INTE knappen där det står *Download .NET Core SDK). Klicka på knappen för att ladda ner installationsfilen. När filen är nedladdad kör du den och följer instruktionerna för att fullfölja installationen. Du behöver inte ändra några inställningar.  

Nu är det dags att installera utvecklingsmiljön. Det är detta program du kommer använda för att skriva kod och för att köra dina egna program när du felsöker koden. Utvecklingsmiljön är heter Visual Studio Code och är gratis. Du laddar ner den från denna [sida](https://code.visualstudio.com/download). Klicka på knappen för nedladdning under operativsystemet på din dator. När filen är nedladdad så kör du den och följer instruktionerna för att fullfölja installationen. 

Efter att du installerat Visual Studio Code kör du programmet på din datorn. Du bör få upp en skärm som ser ut ungefär som nedan, men färgerna kommer se olika ut beroende på dina inställningar. 

<image src="res/2021-01-01-20-03-26.png"/>

Längst till vänster i fönstret för Visual Studio Code finns en area som kallas *Activity Bar* och som ser ut som nedan. 

<image src="res/2021-01-01-20-11-22.png"/>

Ikonerna i denna area öppnar vyer i programmet som används för olika aktiviteter. 

Den första ikonen, som ser ut som två blad, öppnar en vy som heter *Explorer* som hjälper dig överblicka alla filer i ditt programmeringsprojekt. 

Den andra ikonen, som ser ut som ett förstoringsglas, öppnar en vy som heter *Search* och som hjälper dig hitta text i filerna i ditt programmeringsprojekt.

Den tredje ikonen, som ser ut som cirklar med linjer mellan dem, öppnar en vy som heter *Source Control* som hjälper dig versionhantera innehållet i filerna i ditt kodprojekt. 

Den fjärlde ikonen, som ser ut som en skalbagge och en play-knapp, öppnar en vy som heter *Run* som hjälper dig till exempel köra ditt program för felsökning (på engelska kallas felsökning i program för *debugging* och därför säger man ofta *debugga* på svenska istället för felsökning).

Den femte ikonen, som ser ut som fyra kvadratiska klossar, öppnar en vy som heter *Extensions* som hjälper dig att installera utökade funktioner i Visual Studio Code. 

Visual Studio Code kan användas till mycket mer än att bara programmera C# .NET. För att kunna programmera C# .NET med Visual Studio Code måste du innifrån Visual Studio Code installera utökad funktionalitet (eng. *extension*). 

För att installera utökningen i Visual Studio Code, klicka på ikonen för Extension-vyn. Du kommer då få upp en vy i Visual Studio som ser ut ungefär så här: 

<image src="res/2021-01-01-20-26-36.png"/>

I sökfältet högst upp i vyn skriver du ``C#``. Detta kommer resultera i en filtrerad lista av tillgänliga utökningar för Visual Studio Code som har med C# att göra. Efter du skrivit in ``C#`` i sökfältet bör Extension-vyn se ut ungefär så här:

<image src="res/2021-01-01-20-30-13.png"/>

Den utökning du vill installera ligger antagligen högst upp i listan och heter *C#* med *Microsoft* som utgivare. Klicka på den lilla *Install*-knappen till höger om om namnet på utgivaren av utökningen. 

Grattis! Om du lyckats följa instruktionerna ovan så har du nu installerat alla verktyg du behöver för att börja programmera C# .NET. 

Låt oss avsluta genom att skapa ditt första program och samtidigt kontrollera att alla verktygen fungerar som de skall. Börja med att stänga ner Visual Studio Code. 

Det är lämplig att skapa en katalog på din dator där du samlar alla dina programmeringsprojekt. Skapa en sådan var du vill, t.ex. på skrivbordet eller i din hemkatalog. Du kan t.ex. döpa katalogen till ``programmering`` eller ``kod``. Jag har döpt min katalog till ``src``, vilkte är en förkorning av ordet *source* som är engelska för kod. 

I din nya katalog skapar du sedan en underkatalog för ditt första programmeringsprojekt. Kalla denna katalog för ``HelloWord``. 

Öppna sedan upp Visual Studio Code igen. I den stora skärmarean bör du se en länk som heter ``Open folder``. Klicka på länken (ser du inte länken kan du även välja alternativet ``Open..`` under menyn ``File``). Från det nya fönstret som dök upp på skärmen, bläddra fram till katalogen ``HelloWorld`` som du nyss skapade, gå in i katalogen och klicka sedan ``Open``-knappen nere till höger. Ditt Visual Studio Code-fönster bör nu se ut ungefär som på bilden nedan (ser du inte arean med titeln ``EXPLORER``), tryck då på knappen för att öppna Explorer-vyn i din Activity bar. 

<image src="res/2021-01-01-20-48-31.png"/>

I Explorer-vyn, under rubriken ``HELLOWORLD``, ser du alla filer i ditt programmeringspojekt men ännu innehåller inte ditt projekt några filer. 

Det finns många kommandon i Visual Studio Code. Ett enkelt sätt att hitta kommandot man behöver är genom att användra *Kommandopaletten*. Om du kör Windows tryck ``Ctrl`` + ``Shift`` + ``p`` för att få upp kommandopaletten i ditt Visual Studio Code-fönster. Kör du Mac tryck du istället ⌘ + Shift + p. Din fönster bör nu se ut ungefär så här:

<image src="res/2021-01-01-20-58-33.png"/>

Skriv in söktexten ``toggle panel`` efter större-än-tecknet (``>``) i sökfältet tillhörande kommandopaletten högst upp i fönstret. Detta kommer resultera i en filtrerad lista av Visual Studio Code-kommandon under sökfältet. Din skärm bör nu se ut ungefär så här:

<image src="res/2021-01-02-17-56-43.png"/>

Från den filtrerade listan skall du nu välja kommandot ``View: Toggle Panel``. Notera också att till höger om kommandot så står det vilken knappkombination som kan användas som en genväg för att köra kommandot, om det finns någon sådan för det aktuella kommandot. 

Efter att du kört kommandot ``View: Toggle Panel`` dyker ytterligare en vy upp längst ner i fönstret som nu bör se ut ungefär såhär:

<image src="res/2021-01-02-18-01-07.png"/>

Den nya vyn heter *Panel*-vyn och innhåller fyra flikar:
- *Problems*
- *Output*
- *Debug console*
- *Terminal*

Om inte Terminal-fliken är vald i Panel-vyn, välj den nu. 

Terminal-fliken innehåller en terminal där du kan skriva in textkommandot. Terminalen se olika ut beroende på vilket operativsystem du kör och dina inställningar, men fungerar på en grundläggande nivå likadant oavsett utsende. 

Klicka i terminalen och skriv in kommandot: 

```console
dotnet new console
```

Innan du trycker på enter-knappen, bör ditt fönster se ut ungefär såhär:

<image src="res/2021-01-02-18-06-07.png"/>

Tryck på enter-knappen för att verkställa kommandot. 

Efter att du tryck på enter-knappen och kommandot kör färdigt så bör ditt fönster se ut ungefär såhär: 

<image src="res/2021-01-02-18-08-24.png"/>

Kommandot du nyss körde skapade ett programmeringprojekt med alla nödvändiga filer utgående för en mall för *konsolapplikationer*, vilket vi kommer prata mer om senare. Notera i Explorer-vyn att det har dykt upp två nya filer: 
- ``HelloWorld.csproj``
- ``Program.cs``

och en ny underkatalog:
- ``obj``

i katalogen ``HelloWorld`` som du skapade tidigare. 

Du kan klicka på filen ``Program.cs`` för att få din första titt på kod skriven med C# .NET, genererad från mallen. Efter du klickat på filnamnet bör din skärm se ut ungefär så här: 

<image src="res/2021-01-02-18-14-20.png"/>

Första gången du gör detta kommer Visual Studio Code ladda ner paket med funktioner som behövs för att programmera C# .NET. När detta är klart dyker det lilla fönstret som du ser nere till höger i bilden upp. Fönstret ställer frågan:

```console
Required assest to build and debug are missing from `HelloWorld`. Add them?
```

På denna fråga skall du svara genom att trycka på knappen ``Yes`` i det lilla fönstret. Detta kommer göra det lättare att köra och debugga ditt program från Visual Studio Code. 

Klicka igen på Terminal-fliken i Panel-vyn, skriv in kommandot: 

```console
dotnet run
```

och verkställ kommandot genom att trycka på enter-knappen. Om allt fungerade som det skall får du utskriften ``Hello World!`` i terminalen, som i bilden nedan: 

<image src="res/2021-01-02-18-24-29.png"/>

Grattis! Du har lyckats skapa ditt första program med C# .NET! Senare kommer du upprepa processen beskriven ovan men för andra kataloger än ``HelloWorld`` och ändra innehållet i ``Program.cs`` för att ändra hur programmet fungerar. 






