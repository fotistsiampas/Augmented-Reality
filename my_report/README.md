# Lesson: Interaction Design

### First and Last Name: Fotis Tsiampas
### University Registration Number: dpsd17111
### GitHub Personal Profile: https://github.com/fotistsiampas
### Augmented Reality Personal Repository: https://fotistsiampas.github.io/Augmented-Reality/

# Introduction

# Summary


# 1st Deliverable
Αρχικά επειδή δεν είχα αρκετό χώρο στον προσωπικό μου υπολογιστή αποφάσισα να κάνω την εργασία στους υπολογιστές του πανεπιστημίου. Αφού συνδέθηκα με τους κωδικούς μου έψαξα να βρω το github desktop το οποίο δεν είχε εγκατασταθεί ακόμα οπότε αφού κατέβασα και εγκατέστησα το github desktop το άνοιξα και συνδέθηκα με τους κωδικούς του github στην συνέχεια αφού διάβασα προσεκτικά τις οδηγίες έκανα fork το repository. Μετά προσπάθησα να βρω το σωστό path μέσω του powershell αλλά με δυσκόλεψε αρκετά οπότε άνοιξα το command promt και έκανα όλα τα παρακάτω βήματα : 
Z:\>cd “My Documents” (enter) 
Z:\My Documents>cd GitHub (enter)
Z:\My Documents\GitHub>cd Augmented-Reality (enter)
Z:\My Documents\GitHub\Augmented-Reality>python -m http.server (enter)

(Το python -m http.server το βρήκα από το repository merkourisa/Augmented-Reality )
Έπειτα βρήκα μέσα στα discussions το preview του κώδικα και πάτησα [το link](http://localhost:8000) όπου από εκεί πάτησα το marker based και άνοιξε η κάμερα και το μικρόφωνο. Στην συνέχεια πήρα το χαρτί με το hiro και το έβαλα μπροστά στην οθόνη και εμφανίστηκε ο σιέλ κύβος.
Επέστρεψα στο αρχείο του κώδικα στο visual studio για να συμπληρώσω τις νέες εντολές έτσι ώστε να εμφανίζεται ο κύλινδρος και η σφαίρα τις οποίες τις βρήκα από το [διαδίκτυο](https://medium.com/analytics-vidhya/a-frame-changing-environment-tutorial-a71bc69202d4).
<a-entity id="box" geometry="primitive: box; width: 0.3; depth: 0.4; height: 0.3" position="0 0 0"
                          material="color:#f20000 "></a-entity>
                <a-entity id="cylinder" geometry="primitive: cylinder;  height: 0.4; radius: 0.2" position="-0.5 0 0"
                          material="color: #d94c93"></a-entity>
                <a-entity id="sphere" geometry="primitive: sphere; radius: 0.2" position="0.5 0 0"
                          material="color: #306b5d"></a-entity>
Μετά έψαξα τα χρώματα και έβαλα αυτά της επιλογής μου [το σιελ](https://www.google.gr/search?q=%23306b5d&sxsrf=APq-WBsASgSuBRoySP6BXzSmIVxSTL_mYw%3A1647986904515&source=hp&ei=2Eg6YoeiHL2Xxc8Pq8-62AM&iflsig=AHkkrS4AAAAAYjpW6JERSqj_mRp_2scodcO8HRazFedu&ved=0ahUKEwiH7qPQ3dr2AhW9S_EDHaunDjsQ4dUDCAc&uact=5&oq=%23306b5d&gs_lcp=Cgdnd3Mtd2l6EAM6BwgjEOoCECdQug5Yug5gixVoAXAAeACAAYABiAGAAZIBAzAuMZgBAKABAqABAbABCg&sclient=gws-wiz) ,[το ροζ](https://www.google.gr/search?q=%23d94c93&sxsrf=APq-WBvqNHxhCODRhqGuORlFA-E93ZwzHg%3A1647986958533&source=hp&ei=Dkk6YqLMHqH87_UPsPCyiA0&iflsig=AHkkrS4AAAAAYjpXHmdVpLXJjeud4cGo97Adhks_Jl7u&ved=0ahUKEwiii4bq3dr2AhUh_rsIHTC4DNEQ4dUDCAc&uact=5&oq=%23d94c93&gs_lcp=Cgdnd3Mtd2l6EAM6BwgjEOoCECdQ6A9Y6A9gnhloAXAAeACAAZEBiAGRAZIBAzAuMZgBAKABAqABAbABCg&sclient=gws-wiz) [και το κόκκινο](https://www.google.gr/search?q=%23f20000+&sxsrf=APq-WBsBM_TYszTPPnrBIBOjtgzkmHV3Dw%3A1647983115569&ei=Czo6YtGpIsH5kwXIp5LwBA&ved=0ahUKEwiR28vBz9r2AhXB_KQKHciTBE4Q4dUDCA4&uact=5&oq=%23f20000+&gs_lcp=Cgdnd3Mtd2l6EAMyBAgAEB4yBAgAEB4yBAgAEB4yBggAEAUQHjIICAAQBRAKEB4yBggAEAUQHjIGCAAQBRAeMggIABAFEAoQHjIECAAQHjIGCAAQChAeOgcIIxDqAhAnSgQIQRgBSgQIRhgAULIZWLIZYIYgaAJwAHgAgAFriAFrkgEDMC4xmAEAoAEBoAECsAEKwAEB&sclient=gws-wiz)
Εν συνεχεία πρόσθεσα τα χιόνια και τις φωνητικές εντολές start και stop από τους παρακάτω συνδέσμους από το repository που είχα κάνει fork στο Deliverable 1 : [χιόνια](https://www.npmjs.com/package/aframe-particle-system-component) , [φωνητικές εντολές](https://www.npmjs.com/package/aframe-speech-command-component)
και της προσάρμοσα στον κώδικα μου .
<a-entity id="annyang" annyang-speech-recognition></a-entity>
<a-entity id="switch" speech-command__start="command: start; type: attribute; attribute: visible; targetElement: #snow; value: true;"
             speech-command__stop="command: stop; type: attribute; attribute: visible; targetElement: #snow;  value: false;">
</a-entity>
<a-entity id="snow" position="0 6 -15" particle-system="color: #ffffff"></a-entity>

Τέλος πάτησα save στο visual studio για να αποθηκευτούν οι αλλαγές στον κώδικα. Ξανά άνοιξα την κάμερα και αφού πλέον ο κώδικας είχε αλλάξει και είχε ήδη αποθηκευτεί στο github μέσω του github desktop πάτησα refresh και εμφανίστηκαν τα χιόνια στην οθόνη και υψώνοντας το χαρτί με το hiro εμφανιστήκανε και τα σχήματα με το χρώμα που τους είχα δώσει. Εν κατακλείδι με την εντολή stop το χιόνι σταματούσε και με το start (που χρειαζότανε λίγη περισσότερη ένταση ) ξεκινούσε. 




# 2nd Deliverable
Για την υλοποίηση του δεύτερου παραδοτέου εργάστηκα με την ίδια ακριβώς διαδικασία όπως στο 1ο δηλαδή αφού συνδέθηκα στο git hub desktop και άνοιξα το command prompt και έκανα τα παρακάτω βήματα ξανά:
 
Z:\>cd “My Documents” (enter) 
Z:\My Documents>cd GitHub (enter)
Z:\My Documents\GitHub>cd Augmented-Reality (enter)
Z:\My Documents\GitHub\Augmented-Reality>python -m http.server (enter)

Και άνοιξε [η κάμερα](http://localhost:8000) άνοιξα τον κώδικά μου με το visual studio code έψαξα σε διαφορετικά site για να βρώ τουσ κώδικες οι οπιοί θα με βοηθούσαν για την υλοποίηση της εργασίας:

[1ο site](https://stackoverflow.com/questions/61239107/how-to-get-marker-position-x-y-ar-js)

[2o site](https://www.youtube.com/watch?v=XqRVfB521Fo)

[3o site](https://www.youtube.com/watch?v=_HWfc_RqA6k&t=511s)

[4o site](https://www.youtube.com/watch?v=ZYZYnY-uu10&t=198s)

[5o site](https://www.youtube.com/watch?v=MtiUx_szKbI)

[6o site](https://www.w3schools.com/js/default.asp)

[7o site](https://www.w3schools.com/html/default.asp)


Στην συνέχεια αφού με την βοήθεια των παραπάνω ιστοσελίδων αλλά και με την βοήθεια μερικών συναδέλφων κατάφερα να υλοποιήσω τον κωδικά μου πήγα στο [site](https://ar-js-org.github.io/AR.js-Docs/marker-based/) και στην συνέχεια στα [tools](https://ar-js-org.github.io/AR.js/three.js/examples/marker-training/examples/generator.html)
για να φτιάξω τις εικόνες και να τα patterns έτσι ώστε να μπορεί η κάμερα μου να εμφανίζει τις εικόνες και τα τρισδιάστατα αντικείμενα.

Τα τρισδιάστατα αντικείμενα τα επεξεργάστηκα στο πρόγραμμα blender και αφού τα χρωμάτισα με το χρώμα που ήθελα τα έκανα export σε αρχεία gltf ετσί ώστε να είναι υλοποιήσιμα από τον κώδικα μου.

Τέλος αφού αποθήκευσα τον κώδικα στο visual studio code και ανέβασα τισ εικόνες που είχα επεξεργαστεί στα assets όπου όλα είχαν ανεβεί μέσω του github desktop κατέβασα τις φωτογραφίεσ ξανά και στο κινητό μου. Πάτησα refresh και μπροστά από την κάμερα του υπολογιστή έδειξα τις κατάλληκες εικόνες τις οποίες είχα ανεβάσει και στα assets και εμφανίστηκαν τα δύο τρισδιάστατα αντικείμενα στις κάρτες του υδρογόνου και του οξυγόνου ενώ στην κάρτα με το dpsd μου εμφανιζότανε η κατάλληλη εικόνα με το ονοματεπώνυμό μου.

# 3rd Deliverable 


# Conclusions


# Sources
