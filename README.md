pokusao sam napraviti kod za tesitranje prijave za aplikaciju preko unit testa
ima dosta gresaka koje nisam imao vremena ispravljati jer nisam se povezao na firebase
za izradu app i unit testa pratio sam materijale preko kojih smo ucili i istrazivao na interentu

za prvi zadatak se nisam mogao dobro snaci preko beeceptor-a jer nisam na ovakav naci do sada radio sa mock
vec sam prije testirao api samo na postmanu bez beeceptora i mock data
gdje sam radio projveru get,post,put,patch,delete

link za postman: https://www.getpostman.com/collections/a2b1a24c0c69e1e4d2e9

jer nisam najbolje shvatio ovo za postman na ovakav nacin pa cu ovjde napraviti test case za mock data

Tese case Login

Test_Case_ID  Feature    Description          Steps to excute   test data     Excepted result                            Actual result                             Status
    1         button     provjera klika       1.Klik na login                 dobije se poruka da nismo unijeli podatke  dobije se poruka da nismo unijeli podatke PASS
                         na login ako         
                         nismo unijeli
                         kredencijalie
    2        button      provjera kada        1.Unos e-mail-a    e-mail:        dobije se poruka da je lozinka pogresana  dobije se poruka da je lozinka pogresana   PASS
                         unesemo ispravan     2.unos lozinke    career@tech387.com
                         email, a pogresnu    3.klik na log in  lozinka:123dfg!
                         lozinku
                         
    3        button      provjera kada        1.Unos e-mail-a    e-mail:              dobije se poruka da je mail pogresan   dobije se poruka da je mail pogresan    PASS
                         unesemo  neispravan   2.unos lozinke    career@tech.com
                         email, a ispravnu    3.klik na log in  lozinka:Pass123!
                         lozinku
                         
    4        button      provjera kada        1.Unos e-mail-a    e-mail:              uspjesno se logiramo                    uspjesno se logiramo                   PASS
                         unesemo  ispravan   2.unos lozinke    career@tech387.com
                         email i ispravnu    3.klik na log in  lozinka:Pass123!
                         lozinku
