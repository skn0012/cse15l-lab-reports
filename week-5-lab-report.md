# **Week 3 Lab Report - Skyler Nguyen**

## Researching Commands

* I chose the command grep.

## 1. **grep 'string' filename** 

* This searches a specific file that the user inputs for the exact string the user wants (ex. only searches for "Lucayans", not "lucayans"). This includes if the word is part of another word (ex. searching for "an", "and" would be outputted as well). That goes for all the other grep commands. It's useful for searching for a specific string in a specific file.

```
grep "Lucayans" written_2/travel_guides/berlitz2/Bahamas-History.txt

Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.

The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```

```
grep "Bermuda" written_2/travel_guides/berlitz2/Bahamas-History.txt

The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.

In 1648 a group of English Puritans from Bermuda, led by William Sayle, sailed to Bahamian waters and established the first permanent European settlement on the island they named Eleutheria (now Eleuthera) after the Greek word for freedom. The 70 colonists called themselves the Eleutherian Adventurers, but life was very difficult and the colony never flourished, though Sayle was long honored for the effort. In 1666 a smaller island (called Sayle’s island) with a fine harbor was settled by Bermudians and renamed New Providence. It was later to become known as Nassau, capital of the Bahamas.
```


## 2. **grep -i 'string' filename** 

* This searches a specific file that the user inputs for a case-insensitive string that the user wants (ex. both "when" and "When"). It's useful for searching for a string, regardless of capitalization, in a specific file.

```
grep -i "When" written_2/travel_guides/berlitz2/Bahamas-History.txt

English sea captains also came to know the beautiful but deserted Bahamian islands during the 17th century. England’s first formal move was on 30 October 1629, when Charles I granted the Bahamas and a chunk of the American south to his Attorney General, Sir Robert Health. But nothing came of that, nor of a rival French move in 1633 when Cardinal Richelieu, the 17th-century French statesman, tried claiming the islands for France.

When the 13 American colonies, enraged by the Stamp Tax, got into the war that eventually brought independence, the Bahamas somewhat reluctantly found itself on England’s side. But reluctance dissolved as profits from privateering once again flowed into Nassau. This time the plundered vessels were American, but not all the victories were won by the privateers. On 3 March 1776, a rebel squadron under Commodore Esek Hopkins arrived and occupied Nassau for two weeks, a bloodless undertaking that emptied the island’s forts of arms and other military supplies. A smaller and equally non-violent American operation against the town in January 1778 lasted less than three days.

Over the centuries, trouble on the nearby American continent has often meant good news for the Bahamas. When Lincoln ordered a blockade of the southern states in 1861 after the outbreak of the Civil War, the Bahamas quickly boomed. Nassau harbor was busy with ships unloading Confederate cotton and tobacco and taking aboard arms, medicine, and manufactured goods, mainly from Europe, to be run back through the northern blockade. As the war went on, speedy and camouflaged contraband vessels were built to slip past the ever-increasing Federal patrols. Profits from blockade running were incredible, and Nassau went wild. But the extravagant parties and carefree spending stopped abruptly with the North’s victory in 1865. Late the following year an immense hurricane sent a tidal wave over Hog Island (today Paradise Island), smashing Nassau’s flimsy buildings and ruining crops. Other islands were also devastated. As the Bahamas sank back into economic doldrums, citizens turned to agriculture, fishing, or salt raking. The spread of lighthouses and decent navigational charts had crippled the old standby, the wrecking trade.
When the boom suddenly came to an end with the worldwide depression and the repeal of Prohibition in 1933, unemployment rose again, despite the first significant tourism the Bahamas had known.
```

```
grep -i "little" written_2/travel_guides/berlitz2/Algarve-History.txt

Little is known of the earliest Stone Age inhabitants of Europe’s southwestern extremity. The ancient Greeks called them the Cynetes (or Cunetes). Whatever their origins, their culture evolved under the pressure and influence of foreign forces. Among the many invading armies that settled here and contributed to nascent Portuguese culture were Phoenicians, who settled in the area around 1,000 b.c., followed by the Celts, Iberians, Greeks, and Carthaginians.

According to tradition, the site of Prince Henry’s base was the Sagres peninsula (see page 22), though there is little there today to persuade you of this. The actual headquarters of the Navigation School may have been 40 km (25 miles) east, in Lagos (see page 26). This location had a port, shipyards, and was home to the prince in his role as governor of the Algarve.

Among the early blows struck for independence was a rebellion in the town of Olhão (see page 57). On 16 June 1808, the townsfolk — armed with little more than ancient swords, spears, and stones — attacked and captured the local French garrison. It’s said that a party of local men then set sail from Olhão all the way to Brazil, without maps or navigational aids, to tell the king of the insurrection. The real battle, however, was waged under the leadership of the Duke of Wellington, whose coalition forces expelled the French after two years of bitter fighting.
```


## 3. **grep -r 'string' directory** 

* This searches a directory and all of its sub-directories for a specific string. It's useful for searching a whole entire directory for a specific string instead of searching individually.

```
grep -r "Lucayans" written_2

written_2/travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.

written_2/travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.
```

```
grep -r "trident" written_2

written_2/travel_guides/berlitz1/HistoryEdinburgh.txt:        although many strident nationalists thought the proposals did not go

written_2/travel_guides/berlitz1/WhereToItaly.txt:        Nettuno), the burly sea god wields his trident in petrified parody of

written_2/travel_guides/berlitz1/WhereToMalaysia.txt:        range of quite strident regulations governing park usage and duration

written_2/travel_guides/berlitz2/Athens-History.txt:First came Poseidon, who struck the rock of the Acropolis with his mighty trident and brought salt water gushing forth. Then it was Athena’s turn. As she struck the rock an olive tree appeared, which proved more useful and valuable. Thus she acquired the position of the city’s special protector.

written_2/travel_guides/berlitz2/Athens-WhereToGo.txt:Room 15 is dominated by a fine statue of Poseidon in bronze (460 b.c.) found in the sea off the island of Euboea. The god is set to launch his trident against foes unknown. The Hall of the Stairs hosts another statue dredged from the sea, that of the Jockey of the Artemision. The diminutive jockey drives on the handsome steed which has its two front legs raised into the air, as if about to leap over an invisible obstacle.

written_2/travel_guides/berlitz2/Canada-WhereToGo.txt:The true marvel of Niagara is how nature manages to triumph over tawdry commercialism, perhaps less strident on the Canadian than on the American side of the border marked by the Falls. No amount of pushy peddlers or tacky pink honeymoon motels (if you do stay overnight, ask to see one of the hilarious bridal suites) can diminish the spectacle of that mass of white water taking its awesome plunge on the way from Lake Erie towards Lake Ontario and the Atlantic.    

written_2/travel_guides/berlitz2/Nepal-History.txt:Shiva, as Pashupati, is the lord of the animals and the guardian of Nepal. He has 1,008 names in Sanskrit literature. As Mahadev, he is lord of reproduction represented by the lingam, a phallus symbol often appearing in his temples as a stump of stone rising from the female symbol, a disk called the yoni. Shiva is also lord of learning and dance. As bloodthirsty Bhairav, fanged and festooned with skulls, he destroys at will. But he also destroys ignorance and misfortunes — the reason he is the symbol of Royal Nepal Airlines. A statue of Nandi, the bull, and a trident sign mark the temples of Shiva.
```


## 4. **grep -c 'string' filename**

* This searches a specific file and displays the amount of times the string is used in the file. It's useful for finding out how many times a specific string is used in a specific file. 

```
grep -c "Lucayans" written_2/travel_guides/berlitz2/Bahamas-History.txt
2
```

```
grep -c "Bahamas" written_2/travel_guides/berlitz2/Bahamas-History.txt
23
```


## Finding the Source

* I searched up 'how to use grep command in linux' and clicked on the first result.
* This is the [link](https://www.cyberciti.biz/faq/howto-use-grep-command-in-linux-unix/).
