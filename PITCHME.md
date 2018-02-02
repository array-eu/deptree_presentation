
## *Open Source*:

### una consulenza *smart* per una *compliance* integrata

---

## Premessa

### La rivoluzione *<em>embedded</em>  *

- mini computer dotati di sistema operativo (linux)... |
- ...incorporati in dispositivi tradizionali |
  - telefoni, automobili, televisori, frigoriferi, citofoni, videocamere di sorveglianza ecc. |
<li class="fragment">i dispositivi <em>embedded</em>  in circolazione sono il 94%, i PC tradizionali solo il 6% (fonte: [www.wsts.org](https://www.wsts.org), 2010)</li>
<li class="fragment"> lo sviluppo di software <em>embedded</em>  diventa parte integrante del core business di molte aziende "tradizionali" </li>

+++

### Il ruolo dell'*open source*

<span class="fragment"> linux <em>embedded</em>  è cresciuto dal 56.2% nel 2012 al 64.7% nel 2017 (fonte: [www.vdcresearch.com](http://www.vdcresearch.com))</span>
- è ormai uno standard di fatto |
- le ragioni del successo? |
  - motivazioni tecniche e di efficienza di sviluppo |
  - risparmio sui costi di licenza (non c'è una license fee come nel software proprietario) |

---

###  *open source*: gratis non vuol dire "senza condizioni"

- precisi termini da rispettare (diversi da licenza a licenza\), che possono impedire o limitare: |
  - la combinazione di componenti open source tra loro |
  - la combinazione di software open source con software proprietario |

+++

### le conseguenze del mancato rispetto delle licenze

- il mancato rispetto degli obblighi (anche formali) delle licenze open source comporta le medesime conseguenze della violazione delle licenze proprietarie "tradizionali" (tutela del copyright): |
  - inibitorie della distribuzione, descrizioni, sequestri, ecc. |
  - è un rischio concreto (è già accaduto molte volte), specie se i prodotti sono distribuiti a livello internazionale |

---

### i limiti di una consulenza legale tradizionale

- soluzione di singole questioni legali su singoli progetti: |
  - rapida obsolescenza dei pareri forniti (evoluzione del contesto tecnologico e di mercato, e anche del prodotto stesso) |
  - mancata "metabolizzazione" da parte dell'impresa (compliance solo su una singola versione di un prodotto, "dimenticata" nelle versioni successive e nei nuovi prodotti) |

+++

### una consulenza che serve all'azienda

- trasferimento di know-how tecnico-legale |
- la compliance deve diventare parte integrante dei processi aziendali, sopravvivendo al turn-over del personale |
- utilizzo di strumenti software adeguati |
  - per automatizzare alcune fasi del lavoro di compliance |
  - per gestire l'open source policy come wiki aziendale in continua evoluzione |

---

### Il problema, in concreto

- un progetto complesso su piattaforma _<em>embedded</em>_  ha svariate decine di dipendenze da SW di terze parti, include centinaia di pacchetti open source
  - alcune licenze non permettono la combinazione o l’incorporazione in software proprietario |
  - altre sì ma solo a determinate condizioni |
  - altre lo consentono senza particolari problemi |
  - quasi tutte richiedono comunque l'adempimento di alcuni obblighi "formali" |

+++

### Una soluzione *smart*

- una consulenza in cui l'analisi dei singoli progetti software è intrecciata con la redazione di un'open source policy come wiki aziendale aperto |
- l'una procede di pari passo con l'altra |
  - le informazioni acquisite nell'analisi dei singoli progetti vanno riversate nella policy |
  - le procedure definite nella policy vanno testate in tempo reale nelle analisi dei progetti in corso |

---

### Approccio iniziale

- incontro di formazione in azienda |
- sessione con reparto di R&D (progetti in corso e organizzazione interna dello sviluppo) |
- piano di lavoro, si individua un progetto "pilota" |
- analisi del progetto "pilota", in parallelo creazione OSS policy |
- analisi di altri progetti, integrazione dell'OSS policy (sempre WIP) |

<span class="fragment">**tempi e costi si riducono progressivamente, specie se i progetti condividono parti sostanziali**</span>

+++

### L'analisi legale di un progetto software

- freertos: analisi generalmente semplice |
- linux embedded: progetti complessi, da analizzare in quattro fasi |
   - ricostruzione del dependency tree |
   - analisi delle dipendenze software ed individuazione delle criticità legali |
   - individuazione degli adempimenti formali, per i componenti senza criticità |
   - soluzione delle criticità legali individuate |

---

### Strumenti software per l'analisi

<li class="fragment">dependency tree: binary analysis </li>
<li class="fragment"> individuazione ed analisi dei testi legali nei codici sorgenti: [Fossology (http://www.fossology.org)](http://www.fossology.org) </li>
<li class="fragment">i sorgenti non escono mai dall'azienda </li>

+++

### Open source policy

- procedure per il procurement del software open source: regole e criteri per l'inclusione nei progetti aziendali |
- non documento statico ma wiki aziendale in continuo aggiornamento |
- know-how e memoria storica (riutilizzo del lavoro già fatto)|
- fast-track per i casi più comuni |

---?image=assets/images/thanks.jpg
@title[Per approfondimenti]
# Grazie
<div class="bottom">
per approfondimenti:  

[Brevi cenni sull'universo (aperto)](http://www.techeconomy.it/2015/09/11/brevi-cenni-sulluniverso-aperto/)  

[Licenze di software libero e modelli di business](http://www.techeconomy.it/2015/12/04/licenze-software-libero-modelli-business/)  

[Una breve storia personale del software libero (open source)](http://www.techeconomy.it/2015/10/14/breve-storia-personale-software-libero-open-source/)  

[Le licenze di software libero (open source)](http://www.techeconomy.it/2015/11/13/licenze-software-libero-open-source/)  

</div>

---
@title[Copyright e Licenza]
<div class="bottom">
@fa[copyright fa-red] 2018 - Alberto Pianon; Carlo Piana (some rights reserved)   
Licenza Creative Commons by-ND-NC 4.0 unported.  

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.

<p>Presentazione realizzata con [Gitpitch](https://gitpitch.com/) e [Reveal.js][81aa3153]</p>

</div>

  [81aa3153]: https://revealjs.com/ "Reveal"
