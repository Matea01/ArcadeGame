-paddle_height je oznacena kao kosnstranta jer se ne mijenja tijekom igre(osim ako mi ne zelimo nesto promijeniti)
-paddle_height sluzi za postavljanje velicine igračeva reketa. Tako da prakticki ako zelimo otezati ili olasati igracu samo
povecavamo taj broj.
- funkcija koja resetira loptu, pozicionira je u centar ekrana(sirina/
 je chorizontalni centar, isto vrijedi i za visinu. I to cemo posatvljati svaki put kada loptica udari o 
zadnju točku sa desne ili lijeve strane. Ali ovaj dio samo vrati lopticu u centar a ne resetira i smjer kretanja. PA vratimo liniju koda koja to radi.

Dodali smo jos kod koji omogucava da se loptica odbije o reket ako je unutar kooordinata reketa, a ako nije da se resetira pozicija(funkcija)
-kod reketa za drugu stranu postavljamo druge koordinate(1.koordinata je drugacija nego kod prve, to je x os)
-debljina reketa je konstanta pa je postavimo kao const
-radimo isto za reket (rzlika je jedino u broju reketa, vise nas ne zanima paddle1y, nego paddle2y**)
-TEKST NA EKRANU-> canvasContext.fillText
UPDATE SCORE VAR->var player1,2 score. Ako prije lijevu stranu daj lijevome bod(2 igrac), isto i za prvog igraca samo sad esnom stranom
