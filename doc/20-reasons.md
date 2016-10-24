20 reasons why semantic technologies are inefficient... yet?
============================================================

Amazon Alexa, Apple Siri, Facebook M, Google Assistant, Microsoft Cortana. All big companies joined intelligent personal assistant (or virtual assistant) race. Breakthrough? Toy? Yet another kind of interface for search engines? One more attempt to introduce natural language interface to even broader audience? Something in the middle. It is rather an endeavor for introducing semantic technologies into everyday life. Technologies, which try to understand users. But will they succeed? There are serious doubts because virtual assistants mostly work with standard applications and standard areas of searching. So they don't understand everything but mostly only pre-defined areas. What's about third-party applications, user created data, and other areas of searching?

Each virtual assistant optimized for specific area of its creator's concern (e.g. for phones it is voice messages, emails, meetings, etc). Theoretically, third-party applications can use them too through API but the problem is these interfaces are different for each assistant and sometimes are proprietary. Could you imagine if each browser worked with own type of hypertext? Well, to some degree we could, as browsers had specific html tags but finally all competitors agreed it is better to support standards. Why? Because it was a nightmare for developers, when their sites looked differently, and for browser teams, which were constantly requested why this or that page defaced, and, of course, for users, who were disappointed with deformed sites. The same expects virtual assistants unless the situation will change.

Do virtual assistants make difference with what we can do in a browser with search queries? Judging by results, they do not create an additional value for searches. Additionally, they inherit search engine problems. Advertisement and tutorials for intelligent personal assistants mostly focus on standard search areas like maps, directions, weather, stock exchange, entertainment, sports, restaurants. Why? Because they are popular areas for search and, in part, search engines are optimized for queries there. These areas are quite formalized with standard fields/values and therefore we have a lot of sites, which search another N sites of namely these domains. Is search for them ideal? No, because, for example, "hotel room for two near SomeCity center new year" query won't lead you directly to reservations but gives results as if we have "SomeCity hotels" query (further manual filtering required).

20 problems of modern computer semantics
----------------------------------------

If any application is designed to have natural language and give results from files and applications, then, evidently, it needs an interface between natural language and applications. But in what form? And is it possible at all to match applications restricted with assumptions and natural language full with ambiguities? But this is not the only problem as there are more ones, which deeply rooted in the very computer industry and have historical reasons (though some are not viable now). In part, because our interaction with computer is too machine-centric, which can be explained rather by restricted abilities of computer themselves many years ago (but not now). In part, because we accustomed to interact with information namely so and don't want to change our habits.

1. Usage of unique classification. Classification is grouping things by similarity but such grouping is arbitrary as we can have almost infinite number of similarity criteria (for example, "Galaxy -> Solar System -> Jupiter", "Celestial bodies -> Gas giants -> Jupiter", or "Astronomical objects -> Planets -> Jupiter").
2. Classification paths can be confused. We are forced to use file and GUI paths (as a chain of GUI controls and actions with them) but because of arbitrariness we can forget which similarity criteria was used before.
3. Mixed classification/abstraction/specification/inclusivity/relevancy. We can have paths like "SolarSystem/planets/Jupiter/chemistry/reports" though (a) Solar System "has" planets, (b) planet "is class of" Jupiter, (c) Jupiter "relates to" or "has" chemistry, (d) "reports" is rather a summary ("abstraction") of directory content.
4. Duplicate classification. When we copy a file from one place to another, a file path (classification) is not kept always, so, in a new place we are to re-classify it.
5. Not meaningful identification. File names sometimes are encoded (like "jup_meas_2015") or random at all (like "New Document5.txt"). In particular, it occurs because users are not motivated to give meaningful names.
6. Misused or not used abstraction/specification. Though usually it is not underlined but any name should express an aggregated meaning for content. Because users are not motivated to support this, it leads to desynchronization between name and content.
7. Duplicate identification. Very often an internal identification (like a title in a text file) is duplicated with an external identification (in a file name).
8. Scopes are usually static. Thus, directory scope includes files (which are copied or created there) and usually are not present in other scopes (which has different matching similarity criteria for given information).
9. Context is usually interpreted as an ability to have synonyms to words (like "my phone") or dependency on personal data. But we can interpret it wider as it is rather a disambiguation if a given word belongs to the current scope or not (which includes both synonyms and personal data as modifiers of a scope).
10. Semantics is not explicit (for users). For example, hypertext has semantic tags (like "em" instead of "i") but even this tag does not explain why we have emphasis for these words. Another example is relevancy. It is frequently used now but the problem is without knowing relevancy criteria it is hard to use further. The fact "the Sun" is relevant to "nuclear fusion" says us a little about character of this relevancy. Moreover, semantics is not exposed to users as modern semantics approaches assume meaning will be extracted by intelligent agents. Even though no algorithm is able to understand natural language fully and no algorithm is able to summarize content.
11. Users operate with computer entities. For example, we usually operate with "planet file" or "planet database" or "planet window" though in real life we deal with just "planets" but not with "planet book" or "planet model".
12. Meaning enclosed in computer entities. Often meaning is not exposed from UI, binary data, applications, and it is hard to link it between different applications. We can do this only through written instructions, data export, or API but even so meaning remains scattered (as we cut links with other information).
13. Meaning is not considered for user created data. For example, you can create one-time report, which is not worthy of writing an application but which is nonetheless important.
14. Granularity of meaning is often restricted with boundaries of computer entities. But, generally speaking, some meaning scopes may include different parts of several files and some files may include several meaning scopes. Thus, an article about Jupiter may include sections for atmosphere and exploration, which can be considered separately from overall meaning scope of Jupiter.
15. No difference between global search (which is rather "Find me something anywhere") and local search (which is rather "Find me what I lost here").
16. No manual tools for disambiguation and other meaning handling.
17. No automatic tools for disambiguation and other meaning handling.
18. Mostly only top-down approach used in semantics. It forces to define domain entities and rules in "full extent", which is possible only with restrictions and assumptions. Any domain definition can be expanded almost infinitely. Say, if you have "name origin" field for planet table, then you may need to link planet domain with mythology, then with folklore, then with geography, then with biology, then with zoology, etc.
19. Communication is not considered as a part of semantics though it is about information and information update exchange.
20. Natural language questions are not used widely. Though virtual assistants can change this tendency but users are not motivated to do so because search engines have similar results for both "<word>" and "What is <word>" queries, so users may prefer a brief variant.

20 tips for problems of modern computer semantics
-------------------------------------------------

1. Usage of unique identification with classification/abstraction/specification/inclusivity/relevancy behind. It is more or less sufficient to identify Jupiter with "Jupiter" (or "Jupiter (planet)") identifier, if at the same time it is known that (a) Jupiter is in the Solar System, which is in the Galaxy, (b) Jupiter is a gas giant, which belongs to celestial body class of things, (c) Jupiter is a planet, which belongs to astronomical object class, (d) any gas giant is a planet too but not vice versa, (e) celestial body and astronomical object has more or less similar meaning.
2. Any classification path can be used but is not obligatory. You can use any path to reach a target if you forget its name. Or to see similar things by going in the opposite direction from an identifier to wider scopes of meaning.
3. Explicit classification/abstraction/specification/inclusivity/relevancy. This helps to disambiguate similar meaning and make some inference. For example, if Solar System "has" planets and Jupiter "is" planet, then Solar System "has" Jupiter too.
4. Classification should be not duplicated but merged/resolved. For example, you can have one way of "has" based classification on one machine: "Galaxy -> Solar System -> Jupiter", and "is" based one on another: "Celestial bodies -> Planets -> Jupiter". Both machines may communicate and exchange with both variants of classifications because the identifier is the same. On other hand, if settings do not allow classification sharing, then we still can use different classifications as we can operate only with unique enough identifier. These operations do not require user intervention and merging/resolving could be automatic.
5. Meaningful identification must be based on natural language. Therefore, even though you can use "SolarSystem" as a synonym for "Solar System" but generally it is not recommended as we assume any information may be shared with other users and it is quite improbable that many people will look for "SolarSystem" or "Solar_System".
6. Abstraction/specification should be used for identification. For example, if you look for recent Jupiter chemistry report, then it is more probable you look for a document with such summary but not for all documents for which these words are have higher relevancy (for example, it could be an article, which mentions these words).
7. Identification should be done in one place. Therefore, it is possible file names won't be used at all and working with files should be considered as low-level and not user-friendly operation.  Similarly, as ordinary users do not require command line at all (though advanced ones do, of course).
8. Identifiers (meaning) should be considered as both a semantic link and a flexible meaning scope. That is, "Jupiter (planet)" identifier has a meaning behind and any article about Jupiter can be included into its scope. If some text mentions Jupiter the planet, this identifier can be used as a link (similar to a hypertext link but which does not lead to a specific resource). This identifier scope at local computer can be considered as a sort of a directory, which may include items, which are placed here manually (copied/created), items, which are included by inference (search/subscopes/etc).
9. Context is an identifier disambiguation based on a meaning scope. It may help to detect/resolve conflicts with other information. For example, if you have own data on Jupiter chemistry, which does not correspond to other information, then you can override it or mark it as conflicting one.
10. Semantics should be explicit (for users). Explicit semantics will help to disambiguate natural language text to some degree. Though, possibly, we cannot to disambiguate all information completely but at least we can do this for summaries. As for now such disambiguation is not possible without human intervention. For example, search engines give some guesses about meaning of "Jupiter satellites chemistry" but it also may include a reference to a book about alchemy and early modern chemistry (of course, it somehow "relates" to this query but randomly enough). So we need to have rather explicit statement like "planet {is class of} Jupiter {has} satellites {has} chemistry", which can be done by users. They understand semantics from natural language, they work with objects of user interface and file system.
11. [Users may be not aware about computer entities](https://dzone.com/articles/the-next-user-interface-why-how-and-when). They could operate with namely planets. And the fact information saved in a file or information is presented in a window (or how to reach this window) should be implicit and managed by computers.
12. Meaning should be exposed from UI, binary data, and applications. At least, to some degree (as full exposure may contradict with commercial goals). It should be done to make UI, binary data, and applications searchable and integrable with other data and applications.
13. Meaning should be exposed for data created by users. Currently, such data are not considered at all as effort for defining semantics could be inappropriate for one-time task. But if this will be done by the very user, why not?
14. Meaning should cross boundaries of computer entities. For example, a scope of "Jupiter atmosphere" can include only a part of an article about Jupiter and parts of reports on Jupiter chemistry.
15. Local search might won't be required as scopes will be available. In this case, chances to lose our information will be much less.
16. Meaningful text markup should be used to disambiguate identifiers and relations between them. Such markup can be similar to hypertext that will help to keep text clean.
17. Automatic tools for meaning handling may help to choose disambiguated identifiers and markup relations between them, so users may be even not aware about this markup.
18. Both top-down and bottom-up directions in semantics to be covered. Bottom-up approach allows to define meaning in the extent acceptable for you.
19. Communication as an integral part of semantics should be considered as a rather [process of sending notifications](http://dzone.com/articles/is-modern-e-communication-meaningful-enough) than namely information.
20. As natural language questions are rather some meaning with an unknown part, answering is a process of comparing meaning of a question and some domain to identify if there are matches of known and unknown parts. A set of questions and imperative commands may define a natural language interface for applications and data.

How this will work
------------------

Is it clear now how applications can meet natural language? Possibly not, then imagine we look for books about virtual assistants. How this works for applications? An application has API where we can have queryBooks or searchDatabase function with name or bName or bookTitle parameter. How then such API can be used? We need to call queryBooks("virtual assistant"). But wait a minute, is it full match or starting with one? Usually it is documented but could be not expressed through an interface. We have following problems here: (a) names are encoded and sometimes we could only guess if a name is a book name or an author name or if a bName is really book name, (b) another drawback of encoding is we could only theoretically (if developers always follow, say, camel case) decode queryBooks into "query books" but sometimes even decoded phrases are not meaningful, (c) names could be not meaningful enough as searchDatabase, which is rather about internal implementation, (d) we are forced to use only declared function and parameter names and sometimes only in a specific order, (e) it is implied API can be available only through specific protocol or in specific configuration, (g) API and documentation are not integrated, which could help to clarify API usage faster. Of course, sometimes developers follow rules of good naming and names are even meaningful enough. Is it enough? Ideally, such rules should be followed by usage of meaningful names for writing interfaces, which are more or less compatible with natural language. But [no progress here yet](https://dzone.com/articles/the-missing-link-of-software-engineering).

How the same works with natural language queries? It does through "book about virtual assistant" query. Simple? Yes. Working? No. Results are about "Virtual Assistant" series because natural language has one drawback but big one: it is ambiguous. And even if we will add more clarifications with say "book about virtual assistant title", then a search will start to give unrelated results at all. Possibly, we could clarify what user really wants in two-way conversation (as some virtual assistants already do). But can such disambiguation always succeed with ambiguous natural language? Why, if our clarifications with other persons sometimes confuse everything even more? Maybe humans are just not skillful enough to express meaning precisely? No. Vagueness is immanent to abstraction though, of course, we can define strict boundaries as software engineering does (which is not possible in all cases). Therefore, intelligent agents are to use a vague form of knowledge representation (as natural language is). And their clarification could be ambiguous too because to have more or less similar understanding by both parties (humans or machines) we need to have more or less similar definitions. But any definition is based on other definitions so the process of clarification can be recursive and almost infinite. Maybe then parties could operate with the same definitions? No. Because definitions are based on different factors (which can be unknown yet), on context, etc. Therefore, any clarification could be only more or less precise.

No algorithm could resolve our problems with computer semantics. It is barely possible algorithms would understand human texts, which sometimes are unclear for the very humans. There are doubts algorithms would be able to summarize text adequately. Though what we know about adequateness? In fact, each person could summarize the same text quite differently (as different aspects important to him or her). So, what we could expect from algorithms and could we trust them in that? But could we trust humans? Yes, as soon as they will be motivated to make information meaningful and results will be verifiable. And the role of algorithms it support of this. We need efforts in both directions: from computer applications/data to natural language and vice versa with the help of a markup, which may fill a gap between them.  In our example, marked up text may look like "find {} book {abstracts} virtual assistant {is similar} intelligent personal assistant". That is, we (a) separated "find" and "book" and linked them into object-action pair, (b) specified book namely summarizes virtual assistants (but we do not look for a title), (c) disambiguated "virtual assistant" term. Behind scenes, as "find" and "query" can be considered as synonyms and as API call is marked up too, such request may be linked with queryBookBySummary("virtual assistant"). What algorithms may help to do is (1) to disambiguate identifiers (similarly, as they already do in search controls and some sites), (2) to construct markup so it will be transparent for users (for example, with two-way conversation but which focused on specifying relations).