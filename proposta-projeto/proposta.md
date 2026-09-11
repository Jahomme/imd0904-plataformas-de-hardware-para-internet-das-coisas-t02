# Proposta de Projeto: Monitor de Umidade do Solo Automatizado (Horta Inteligente)

### Contextualização do Problema
Pessoas que viajam com frequência ou esquecem a rotina de irrigação doméstica enfrentam perdas constantes de plantas por dessecação ou apodrecimento das raízes causado pelo excesso de água. A falta de monitoramento contínuo inviabiliza uma rotina de cuidados eficiente e equilibrada.

---

### Especificação de Hardware

* **Controlador Central:** 1x ESP32 (comunicação Wi-Fi integrada).
* **Sensoriamento:** 1x Sensor Capacitivo de Umidade do Solo (maior durabilidade contra corrosão por oxidação comparado ao modelo resistivo).
* **Atuador e Acionamento:** 1x Mini bomba d'água submersível (5V) + 1x Módulo Relé isolador (ou 1x LED indicador para fins de bancada/simulação).

---

### Arquitetura de Funcionamento e Integração IoT

* **Aquisição de Dados:** O ESP32 realiza leituras periódicas do sensor capacitivo em intervalos pré-programados de tempo.
* **Transmissão e Nuvem:** Os dados de umidade são enviados via Wi-Fi para um broker IoT (como Adafruit IO).
* **Lógica de Controle:**
  * **Modo Automático:** Se a leitura de umidade for inferior ao limite definido (ex.: $< 30\%$), um sinal de acionamento é disparado para armar o relé e ativar a bomba de irrigação.
  * **Modo Manual/Remoto:** O usuário monitora o nível em tempo real através de um painel de controle (Dashboard) e pode acionar a bomba manualmente à distância via internet.

