# Photon ↔ Helium — model interakcji

Repozytorium opisuje **rolę fotonu** w procesach związanych z **atomem helu**:

- do czego potrzebny jest foton,
- jakie energie są wymagane,
- jakie długości fali z tego wynikają,
- jak to przeliczyć na poziomie: 1 atom ↔ 1 mol ↔ wiązka fotonów.

---

## 1. Założenia fizyczne

Pracujemy na **atomie helu w fazie gazowej**.

### 1.1. Energie jonizacji helu

- **Pierwsza jonizacja He → He⁺ + e⁻**  
  \(E_1 \approx 24.59\ \text{eV}\)  
- **Druga jonizacja He⁺ → He²⁺ + e⁻**  
  \(E_2 \approx 54.42\ \text{eV}\)  
- **Całkowite usunięcie obu elektronów**  
  \(E_{\text{tot}} = E_1 + E_2 \approx 79.01\ \text{eV}\) 

---

## 2. Rola fotonu

Foton jest:

- **nośnikiem energii kwantowej**:  
  

\[
  E = h \nu = \frac{hc}{\lambda}
  \]


- **wyzwalaczem przejścia**:  
  jeśli \(E_{\gamma} \ge E_{\text{prog}}\), może:
  - wzbudzić atom,
  - zjonizować atom (wyrwać elektron),
  - doprowadzić do pełnej jonizacji (He → He²⁺). 

Hel jest tu **medium / obiektem**, foton jest **kluczem energetycznym**.

---

## 3. Obliczenia progowych długości fali

Używamy:


\[
E = \frac{hc}{\lambda}
\quad\Rightarrow\quad
\lambda = \frac{hc}{E}
\]



Stałe:
- \(h = 6.62607015 \cdot 10^{-34}\ \text{J·s}\)
- \(c = 2.99792458 \cdot 10^{8}\ \text{m/s}\)
- \(1\ \text{eV} = 1.602176634 \cdot 10^{-19}\ \text{J}\)

### 3.1. Pierwsza jonizacja He

- \(E_1 = 24.59\ \text{eV}\)
- W dżulach:
  

\[
  E_1^{(J)} = 24.59 \cdot 1.602176634 \cdot 10^{-19}
  \approx 3.94 \cdot 10^{-18}\ \text{J}
  \]


- Długość fali progowej:
  

\[
  \lambda_1 = \frac{hc}{E_1^{(J)}}
  \approx \frac{6.626\cdot 10^{-34} \cdot 2.998\cdot 10^{8}}{3.94\cdot 10^{-18}}
  \approx 5.04 \cdot 10^{-8}\ \text{m}
  \approx 50.4\ \text{nm}
  \]


Region: **daleki ultrafiolet (EUV)**. 

### 3.2. Druga jonizacja He⁺

- \(E_2 = 54.42\ \text{eV}\)
- W dżulach:
  

\[
  E_2^{(J)} = 54.42 \cdot 1.602176634 \cdot 10^{-19}
  \approx 8.72 \cdot 10^{-18}\ \text{J}
  \]


- Długość fali progowej:
  

\[
  \lambda_2 = \frac{hc}{E_2^{(J)}}
  \approx 2.28 \cdot 10^{-8}\ \text{m}
  \approx 22.8\ \text{nm}
  \]



### 3.3. Całkowita jonizacja (He → He²⁺ jednym fotonem)

- \(E_{\text{tot}} \approx 79.01\ \text{eV}\)
- W dżulach:
  

\[
  E_{\text{tot}}^{(J)} \approx 79.01 \cdot 1.602176634 \cdot 10^{-19}
  \approx 1.27 \cdot 10^{-17}\ \text{J}
  \]


- Długość fali progowej:
  

\[
  \lambda_{\text{tot}} = \frac{hc}{E_{\text{tot}}^{(J)}}
  \approx 1.57 \cdot 10^{-8}\ \text{m}
  \approx 15.7\ \text{nm}
  \]



---

## 4. Skala: 1 atom ↔ 1 mol ↔ wiązka fotonów

Liczba Avogadra:


\[
N_A = 6.02214076 \cdot 10^{23}\ \text{mol}^{-1}
\]



### 4.1. Energia na 1 mol helu (pierwsza jonizacja)



\[
E_{1,\text{mol}} = E_1 \cdot N_A
\]



W jednostkach chemicznych:


\[
E_{1,\text{mol}} \approx 24.59\ \text{eV} \cdot 96.485\ \frac{\text{kJ}}{\text{mol·eV}}
\approx 2370\ \text{kJ/mol}
\]



### 4.2. Liczba fotonów potrzebnych do zjonizowania 1 mola

Jeśli każdy foton ma energię dokładnie \(E_1\):

- **1 foton na 1 atom**  
- **\(N_A\) fotonów na 1 mol**

Jeśli foton ma energię większą niż próg, nadwyżka idzie w energię kinetyczną elektronu.

---

## 5. Do czego był potrzebny foton (w tym modelu)?

1. **Do przekroczenia progu energetycznego**  
   Bez fotonu o odpowiedniej energii elektron pozostaje związany.

2. **Do selektywnego sterowania stanem helu**  
   - foton o energii < \(E_1\) → tylko wzbudzenia, brak jonizacji,  
   - \(E_1 \le E_{\gamma} < E_2\) → możliwa pierwsza jonizacja,  
   - \(E_{\gamma} \ge E_2\) (lub suma fotonów) → możliwa druga jonizacja.

3. **Do kodowania informacji w stanie helu**  
   - stan He / He⁺ / He²⁺ może być traktowany jako **nośnik stanu logicznego / informacyjnego**,  
   - foton jest **operatorem zmiany stanu** (write / flip / erase).

---

## 6. Ustalenia do repo

- Hel jest **nośnikiem stanu** (medium).  
- Foton jest **kwantowym sygnałem sterującym** (trigger).  
- Wszystkie progi energetyczne są policzone i podane:
  - \(E_1, \lambda_1\) — pierwsza jonizacja,  
  - \(E_2, \lambda_2\) — druga jonizacja,  
  - \(E_{\text{tot}}, \lambda_{\text{tot}}\) — pełna jonizacja jednym fotonem.  
- Skala molowa i liczba fotonów są jawnie zdefiniowane.

- # 7. Helisa fotonu, jego widmo i czas jako struna

W tym modelu foton **nie jest punkowym „pakietem energii”**, tylko:

- **helisą** (skręconą strukturą fazową),
- **widmem** (ciągiem częstotliwości, nie jedną),
- **struną czasową** (czas nie jest osią, tylko rozciągniętą strukturą).

To oznacza:

## 7.1. Foton jako helisa
Foton ma:
- kierunek propagacji,
- skręt (helicity),
- fazę,
- amplitudę,
- częstotliwość.

W tym modelu skręt = **geometria informacji**.  
Helisa = **nośnik orientacji**.

Dlatego foton może:
- przenosić informację,
- zmieniać stan obiektu (np. helu),
- inicjować przejścia energetyczne.

## 7.2. Foton jako widmo
Każdy foton ma:
- częstotliwość dominującą,
- ale także **widmo boczne** (harmoniczne).

To widmo decyduje:
- czy trafi w próg jonizacji,
- czy wzbudzi atom,
- czy przekaże nadwyżkę energii elektronowi.

Widmo = **sygnatura fotonu**.

## 7.3. Czas jako struna
W szczególnym przypadku (gdy foton jest analizowany w czasie):

- czas nie jest linią,
- czas jest **struną** — rozciągniętą helisą fotonu.

To pozwala:
- analizować rezonans,
- badać zgodność fazową,
- rozumieć emergencję stanu.

To jest kluczowe dla:
- rezonansu,
- stabilności,
- powstawania nowych stanów.

---

# 8. A co z helem?

Hel w tym modelu pełni **trzy role**:

## 8.1. Hel jako medium testowe
Hel jest:
- prosty (2 elektrony),
- stabilny,
- dobrze opisany,
- ma wysokie energie jonizacji.

Dlatego jest idealny jako:
- obiekt testowy,
- nośnik stanu,
- „pamięć kwantowa”.

## 8.2. Hel jako odbiorca fotonu
Foton jest **operatorem zmiany stanu**,  
a hel jest **obiektem, który ten stan zmienia**.

Foton może:
- wzbudzić hel,
- zjonizować hel,
- podwójnie zjonizować hel.

To daje trzy poziomy stanu:
- He (neutralny),
- He⁺ (1 elektron),
- He²⁺ (jądro).

To są **stany logiczne**.

## 8.3. Hel jako stabilizator informacji
Hel po jonizacji:
- jest stabilny,
- nie rozpada się,
- nie reaguje chemicznie.

Dlatego stan He / He⁺ / He²⁺:
- jest trwały,
- jest mierzalny,
- jest powtarzalny.

To czyni hel **idealnym nośnikiem informacji**.

---

# 9. Dlaczego foton był potrzebny?

Bo tylko foton może:

1. **przekroczyć próg energetyczny**  
   - 24.59 eV → He → He⁺  
   - 54.42 eV → He⁺ → He²⁺  
   - 79.01 eV → pełna jonizacja jednym fotonem

2. **przenieść orientację (helisę)**  
   Hel nie zmieni stanu sam z siebie — potrzebuje operatora.

3. **zsynchronizować czas (strunę)**  
   Rezonans wymaga zgodności fazowej.

4. **wprowadzić informację**  
   Foton = sygnał sterujący.

---

# 10. Wszystkie obliczenia (zebrane w jednym miejscu)

## 10.1. Energie jonizacji helu
- \(E_1 = 24.59\ \text{eV}\)
- \(E_2 = 54.42\ \text{eV}\)
- \(E_{\text{tot}} = 79.01\ \text{eV}\)

## 10.2. Długości fali progowe


\[
\lambda = \frac{hc}{E}
\]



- \(\lambda_1 \approx 50.4\ \text{nm}\)
- \(\lambda_2 \approx 22.8\ \text{nm}\)
- \(\lambda_{\text{tot}} \approx 15.7\ \text{nm}\)

## 10.3. Energia molowa


\[
E_{1,\text{mol}} \approx 2370\ \text{kJ/mol}
\]



## 10.4. Liczba fotonów
- 1 foton → 1 atom  
- \(N_A\) fotonów → 1 mol  

---

# 11. Finalne ustalenie modelu

- Foton = **helisa + widmo + struna czasu**  
- Hel = **nośnik stanu + stabilizator + odbiorca**  
- Interakcja = **zmiana stanu przez przekroczenie progu energetycznego**  
- Rezonans = **zgodność fazowa fotonu i odpowiedzi helu**  
- Emergentny stan = **He / He⁺ / He²⁺ jako zapis informacji**


