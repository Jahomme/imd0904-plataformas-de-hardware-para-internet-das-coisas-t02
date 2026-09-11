## Experimento 01: Polarização Direta versus Polarização Reversa de Diodos

* **1. Comportamento do LED:**
  * **[Link Falstad](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiAzABwBMuA7AGw1G1IAsFAnF9o+6hAAjREWyoADiISdUANwijUAW0yiApgFokKAHwAoKFGByoAD0T8oFCoyhWkjcbESPUAd3gJnygIZm5JQB6AyNgd3NLdihHbBikGhinVC9xEMNjABNI5ASkuKQmfJScFQB7REz1GF8AVwAbNAR0sIiLZCLYqBoaaNiS72bQ4zbEHr6nbt6YrhoBtOHgaHbxmcTVlkZ51EVkQiGM4AAZAFEAERyNojtVmy2XQahlCoQqmoa0TXr1TMFdlCgIAA5qVAdIfEJyN58CgWiMclY7lNondtulgEFwBADEA)**
  * **Comportamento:** O led ascende.

---

* **2. Tensão sobre o Resistor de 1kΩ:**
  * **Valor Medido (Simulado):** O valor medido foi de V = 2.835 . O valor foi menor que 5V pois, quando liga o led em serie com o resistor e o diodo, a tensao em cada componente divide, e a tensao total do circuito é a soma.
---

* **3. Cálculo da Corrente e Comparação:**
  * **Cálculo Teórico:**
    $$V_R = V_{fonte} - V_{diodo} - V_{LED} = 5 - 0{,}7 - 1{,}7 = 2{,}6\text{ V}$$
    $$I = \frac{V_R}{R} = \frac{2{,}6\text{ V}}{1000\,\Omega} = 0{,}0026\text{ A} = \mathbf{2{,}6\text{ mA}}$$
  * **Valor Medido no Simulador:** **$2{,}835\text{ mA}$**
  * **Comparação:** O valor medido (2,835 mA) é muito próximo do teórico (2,6 mA). A pequena diferença acontece porque usamos valores fixos no papel (0,7V e 1,7V), enquanto no simulador a queda de tensão real dos diodos varia de acordo com a corrente do circuito, ficando ligeiramente menor que as médias teóricas e deixando passar um pouco mais de corrente.
---

* **4. Comportamento do LED:**
  * **[Link Falstad (Figuras 2 e 3)](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiAzABwBMuA7AGw1G1IAsFAnF9o+6hAAjREWyoADiISdUANwijUAW0yiApgFokKAHwAoKFGAB3KAA9EmikRpQK2dlG1c7DgbBwIA9AaPAAGQBRABELKyRXKBZGZ0i3R1R4BHEoZQB7RAATdRgAQwBXABs0TSL1LMFFZEEAcy8oYQblIXIU-BRfQ2NoSwQXOw4nAeiiRiSG6qRCHz9jMz6RpBoqOKihiZTZ7tNw-pp2bChl1aWVzfEu-yy960djlecDo5OLlUyEHPzitG3-BasNkGjzuTleni2V2McluQIepzh7k2SHGUBMyVSyjy5jkSihwBhiyoLxBxPsiQhKNQ6Oa2NxCBI+IB-TJJ2cFGBVDeTNhnKgrPOEMuc12fQFq1Z7A8GL+PT2kqcZJibygUxm+OCYTFR3c-KOyqF72yuUKJTKFSqiBQjXqW0a0kxrRwHVloqsZN1HopMp5fSQTHh0QO8O5IpufRowbZK1W4JlaQ+X1Nv19iBjgYoFFica8qYQmezjwLxyloZ2vUoWeOjB1VeeKrVBFdmr2xZi9irSMNCeN3zN5UqjSmdQaTTtLTaeGwnRFzP9sV1xa7PpFhKtAd185DlNRNJqsGHaTpSigQjAeSwDNdzOLKNr2dLhrzt5rUEOLxrZf+rbrhw7sQNFcdhvX8jnfaJDi-YwJD2cC7zfAgINSZIKBUdQGgwSdUAgdDkEIfDtmAbxwAgAwgA)**
  * **Comportamento:** O led permanece apagado.
---

* **5. Diferença entre os Circuitos de Polarização (Item 1 vs Item 4):**
  * Na **polarização direta** (Item 1), o diodo está na posição correta e deixa a corrente passar, fazendo o LED acender.
  * Na **polarização reversa** (Item 4), o diodo está invertido e bloqueia a corrente como se o circuito estivesse aberto, mantendo o LED apagado. O diodo só deixa a energia passar em um sentido.

---

* **6. Circuito sem o Diodo:**
  * **Houve diferença?** Sim. O LED acende.
  * **Motivo:** O diodo que estava invertido e bloqueando a corrente foi removido. Sem essa barreira no sentido contrário, o circuito fecha normalmente e permite a passagem de corrente para acender o LED.

---

* **7. Circuito com Fonte CA (Senoidal 5V pico, 1Hz):**
  * **a. Comportamento e Frequência do LED:** Sim, o LED pisca. Ele acende 1 vez por segundo.
  * **b. Tensão no Resistor durante o Semiciclo Negativo:** A tensão no resistor cai para 0 V. Isso ocorre porque, quando a tensão fica negativa, a polaridade se inverte e o diodo fica polarizado reversamente, bloqueando a corrente e deixando o circuito aberto.


## Experimento 02: Portas lógicas com Diodos

* **1. Comportamento Porta Lógica:**
  * **[Link Falstad](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiAzABwBMuA7AGw1G1IAsFAnF9o+6hAAjREWyoADiISdUANwijUAW0yiApgFokKAHwAoKFGByoAD0Saa7bFCRcaUKzahdGqeMndQA7p-FQygCGZnJKAPQGRsA+5pbWtm5OCVBUAf4IkYbGsRYIzrZpTkhMqek4mVE5cfkpFI7apfUeFVnRufEu9g0pNPQ0LQjibdV5BVB9jkiME-2Dw1UxNdOzUzMJ85XZS3kr7FR2M26bI8AA5jWNMxTY7MVNFN4Zp9C7RzMr0+VDqIrIhFtogAZACiABFlh9GLYVhtYBVAgB7RAAE3UMCCAFcADZoTTY9QowR-FBQEBnBHCBHKITkIb4FCnFGXJL7Q5QfabJGo9FY3GA4zMsZJJIrY7wn7chBojE4tACnaWVkHbQ0A6ciULbYdfIlGb8e7XW4nRY6zQimaqg7i56my4pIrjZqahUAZUuSDVHJVeu9XOxYARaAAFogBqd3WNPdbLb6bQiA0HQwhwwZgOFwBADEA)**

---

* **2. A alteração das chaves SW1 e SW2 :**
  * **Comportamento LED como porta lógica:** O circuito realiza a operação lógica OR porque o LED acende (nível lógico 1) se **qualquer uma** das chaves estiver na posição 2 (+5V), ou se **ambas** estiverem na posição 2. Ele só permanece apagado (nível lógico 0) quando ambas as chaves estão na posição 1 (0V).
---

* **3. Comportamento Porta Lógica:**
  * **[Link Falstad](https://www.falstad.com/circuit/circuitjs.html?ctz=DwYwlgTgBAZgvAIgIwKgFwM6IAwDpsEECsqYIiAzABwBMuA7AGw1G1IAsFAnF9o+6hAAjREWyoADiISdUANwijUAW0yiApgFokKAHwAoKFGByoAD0Sb+UJFxpRNNdtht3U8ZI1QB3D+KjKAIZmckoA9AZGwN7mlta29jqJbrA4CBGGxjEWyEjJiXk2NFTuaRlR2ZZOLgkO1VD8pQji5cbQOdqMLtaOzg0Cqc2oisiE6ZFZsQid3ewOSf1NLRPRUwt5VDaFjYPLmcAAMgCiACJTFPZcjFuXXrsqAPaIACbqMIEArgA2aJpf6s9BCMUFAQABzNKg6T+ZRCcjNfAoVrAADKU202zmVjmOz8kkQIK+YEhaAAFogaON9s90dYqC4XPSlo8Xm9Pj8qRVaXN2JsXLzmcjKrl7NYLot7si0TlGS5xUz7lAJATUESSeSEJShVN+ZtxbiygZgGFwBADEA)**

---
* **4. A alteração das chaves SW1 e SW2:**
  * **Comportamento LED como porta lógica:** O circuito realiza a operação lógica AND porque o LED em teoria acende (nível lógico 1) se **ambas** das chaves estiver na posição 2 (+5V). Ele só permanece apagada (nível lógico 0) quando quando pelo menos uma das chaves está na posição 0 (0V). 
  * **OBS:** Meu led não ascendeu não sei exatamente por que, mas pela lógica o comportamento seria de uma porta lógica AND.