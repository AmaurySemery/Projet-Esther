# Projet-Esther
Conception d'un robot-araignée intelligent

# Objectifs

Mes objectifs sont par étapes les suivants :
* Choisir un système de servo/châssis qui ait le potentiel de donner une fluidité, agilité, puissance satisfaisante pour donner aux mouvements d'Esther un côté réaliste
* Choisir une carte électronique adaptée aux nombres et aux types de servos choisis, qui puisse accueillir les différents capteurs et la connectivité Wifi/4G
* Concevoir un système de détection des obstacles par ultrason/infrarouge pour simuler le sens visuel
* Concevoir une caméra pour plus tard accueillir un éventuel programme de détection visuel par Deep Learning [facultatif]
* Concevoir un système de détection des sons pour simuler le sens auditif
* Concevoir un système de détection de l'organique par les pattes pour simuler le sens du toucher [facultatif]
* Concevoir un système de communication par les mots avec un afficheur LCD
* Concevoir un système de communication émotionnel avec des couleurs de led différentes pour les pupilles et éventuellement des sourcils gérés par des servos
* Trouver une solution pour gérer la puissance et donner une autonomie satisfaisante à Esther (batterie, moteur, etc.)
* Travailler la programmation pour mettre au point un mode de déplacement basique
* Mettre au point plusieurs autres modes de déplacement (pour simuler des émotions, comme l'empressement, la peur, la timidité, la colère, etc.)
* Programmer des gestuelles particulières (comme saluer, pousser un objet, taper dessus, donner la patte, faire le beau, etc.)
* Programmer des réactions suivant des stimulis physiques (claquer des mains, toucher le robot, montrer un objet qui excitera les sens infrarouges, etc.)
* Connecter la carte électronique à un serveur en ligne qui accueillerait des codes python pour augmenter les facultés d'apprentissage d'Esther
* Programmer des danses qui dépendraient de la détection auditive de quelques musiques
* Rendre Esther autonome avec une attitude émotionnelle randomisée par le programme ou dépendant de stimulis physiques donnés
* Développer ce dernier aspect en concevant un caractère pour Esther
* Mettre au point des punchlines sur l'afficheur LCD

# Châssis

* [20DOF Aluminium Hexapod Robot araignée Six jambes Robot bras cadre Kit pour Arduino bricolage](<https://fr.aliexpress.com/item/32757236180.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-1&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [Kit de cadre Robot en Aluminium hexapode araignée Six 3DOF jambes avec roulements pour Arduino bricolage](<https://fr.aliexpress.com/item/32757326561.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-2&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [1 ensemble Arduino alliage d'aluminium Hexapod Spider Six 3DOF jambes Robot cadre Kit livraison directe au détail + livraison gratuite](<https://fr.aliexpress.com/item/32646972277.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-8&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [Adeept Hexapod araignée Robot Kit tige robotique Kit pour Arduino cerveau-formation jouet pour enfants enfant jouets éducatifs cadeau d'anniversaire](<https://fr.aliexpress.com/item/1005001303840556.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-10&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [Bouclier de capteur de Robot Arduino à Source ouverte Six Led SG90 servomoteur bricolage programme étudiant Kit de tige de projet](<https://fr.aliexpress.com/item/4001101178830.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-12&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [Kit de support de Robot araignée Hexapod classique kit de support en alliage d'aluminium à Six pattes 18DOF-sans Servos](<https://fr.aliexpress.com/item/4000968131866.html?spm=a2g0o.detail.1000014.33.21c6db61sCoSWI&gps-id=pcDetailBottomMoreOtherSeller&scm=1007.14976.190395.0&scm_id=1007.14976.190395.0&scm-url=1007.14976.190395.0&pvid=2faed1f4-b8ff-41e2-988c-1f5af46fd4b3&_t=gps-id:pcDetailBottomMoreOtherSeller,scm-url:1007.14976.190395.0,pvid:2faed1f4-b8ff-41e2-988c-1f5af46fd4b3,tpp_buckets:668%230%23131923%2348_668%23808%233772%23906_668%23888%233325%2316_4976%230%23190395%2318_4976%232711%237538%2382_4976%233104%239653%237_4976%234052%2318550%2347_4976%233141%239887%234_668%232846%238109%23252_668%232717%237563%23547_668%231000022185%231000066059%230_668%233422%2315392%23807_4452%230%23184418%230_4452%233474%2315675%2369_4452%233098%239599%23242_4452%233564%2316062%23585>)
* [Arduino UNO R3 araignée Robot capteur bouclier quatre Led SG90 Servo contrôle bricolage étudiant projet Kit](<https://fr.aliexpress.com/item/4000421910110.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-17&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [Hexapod Robot araignée Robot rampant PS2 contrôle 25kg équipement de direction en métal Code Source libre pour Arduino bricolage tige programme jouet Kit](<https://fr.aliexpress.com/item/4001241267818.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-22&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [Avec MG996R Servos et contrôleur ensemble complet pour Arduino bricolage RC jouet 18DOF Aluminium Hexapod araignée Six jambes Kit Robot](<https://fr.aliexpress.com/item/32759587711.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-20&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [Bricolage Hexapod bionique araignée Robot Kit Intelligent Programmable haute technologie KEXUE enfants jouets éducatifs](<https://fr.aliexpress.com/item/32966213532.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-25&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
* [20DOF Kit de cadre Robot en Aluminium Hexapod Robot araignée Six jambes Compatible avec Arduino](<https://fr.aliexpress.com/item/32781166310.html?spm=a2g0o.productlist.0.0.c23c16f7wi7GCA&algo_pvid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf&algo_expid=6a6bd7c0-9b87-4769-a313-1d8d2317a3cf-27&btsid=0b0a187b16011122705956414e4435&ws_ab_test=searchweb0_0,searchweb201602_,searchweb201603>)
