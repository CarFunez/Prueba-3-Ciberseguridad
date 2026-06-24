# Prueba-3-Ciberseguridad
Riesgos y amenazas de los sistemas y la red 
ITEM 1:Configuración básica de un firewall de filtrado de paquetes 

Verificar la conectividad:
Lo primero que hice fue verificar la configuración de red del equipo. Se comprobó que el dispositivo perteneciera a la red 192.168.56.0/24, permitiendo la comunicación entre el sistema Windows anfitrión y la máquina virtual Kali Linux. 
<img width="903" height="509" alt="{9EE1EBE9-2492-4DE6-BD10-3F7BDBDA87B0}" src="https://github.com/user-attachments/assets/d7cc3c6c-3a75-4cf4-9521-56eafd94631b" />
Prueba de conectividad entre Windows y Kali Linux. 
<img width="902" height="508" alt="{54259CA1-6C3E-4B82-B143-AF07E003B499}" src="https://github.com/user-attachments/assets/8f0e5776-58de-455b-a200-4c2d41eae297" />
Instalación y configuración del servicio SSH y apache2
<img width="900" height="272" alt="{1ACA48F8-738D-47EA-9A06-37DBF3329292}" src="https://github.com/user-attachments/assets/246650b6-ec36-4308-96e1-97903805f365" />
Estado operativo del servicio Apache2:
<img width="901" height="287" alt="{0D0D086C-2E2E-46EE-B6F4-EF208183AB2A}" src="https://github.com/user-attachments/assets/c8e8a0ea-a2d1-4f53-9eb4-40a29d423871" />
Acceso exitoso al servicio HTTP desde el cliente Windows. 
<img width="907" height="510" alt="{73E38EAC-27F5-4FA2-878E-2A99D9C9CBAD}" src="https://github.com/user-attachments/assets/186b2f26-2775-46d3-b9ce-f79312db14b9" />
Implementación del firewall nftables:
Luego de habilitar los servicios requeridos, se procedió a instalar nftables como mecanismo principal de filtrado de tráfico. Se configuró una política de seguridad restrictiva basada en el principio de mínimo privilegio, permitiendo únicamente el tráfico necesario para el funcionamiento de los servicios autorizados. 
<img width="904" height="508" alt="{FF0185E8-BD0E-4C77-87C5-C3325A661D52}" src="https://github.com/user-attachments/assets/1aafae5f-cb84-49eb-be59-807418e69fe8" />
Acceso al servidor Apache a través del navegador web: 
<img width="902" height="504" alt="{D74833B5-C305-42F1-9210-28EA5880FFE0}" src="https://github.com/user-attachments/assets/43a0ce38-7d94-4c77-af90-f9e3faa05d49" />
Conexión remota segura mediante SSH. 
<img width="897" height="499" alt="{83124F7A-A5E2-45EB-9643-EB68F356A5AF}" src="https://github.com/user-attachments/assets/566cc21c-c8ce-4dbf-a6bf-05bd925f6b88" />
ÍTEM 2: IMPLEMENTACIÓN DE IDS MEDIANTE SURICATA 
instalación de suricata
Como segunda etapa de la actividad se implementó un Sistema de Detección de Intrusiones utilizando Suricata. Se realizó la instalación del software y posteriormente se verificó la versión instalada mediante comandos de validación. 
Instalación y verificación de Suricata. 
<img width="898" height="506" alt="{9185AB0C-5981-4F21-8696-BD4B11725DBD}" src="https://github.com/user-attachments/assets/344205c1-3d8e-418d-b0a9-d7d60d629f6d" />
<img width="900" height="506" alt="{4F375697-ABBA-45DA-A632-6A2B0D599519}" src="https://github.com/user-attachments/assets/0bae0fa2-a52c-47aa-bdf9-bc508c3356b2" />
<img width="900" height="505" alt="{05E75FC0-2DF6-4D37-87C4-CCF7547307A8}" src="https://github.com/user-attachments/assets/9058df8b-52ee-4139-b3f3-c2728a5ee557" />
Configuración de HOME_NET en el archivo suricata.yaml. 
<img width="902" height="735" alt="{E92A8466-7567-4C87-8F09-4B283D1C14F0}" src="https://github.com/user-attachments/assets/598bf808-f457-42b3-8c43-ca859a2d1632" />
<img width="905" height="504" alt="{44568C6C-31D5-45BE-AD8B-ACCA56509E20}" src="https://github.com/user-attachments/assets/e9013e04-aac2-4dd7-9eff-6c6c0c7666c7" />
Actualización de reglas mediante suricata-update. 
<img width="899" height="428" alt="{35326D83-8867-44B7-B118-6388F5B7CDF0}" src="https://github.com/user-attachments/assets/73c5691d-1013-4f28-924f-c1cdc6f8b3a0" />
<img width="903" height="507" alt="{8833FA80-284B-407E-8FA7-23233E693668}" src="https://github.com/user-attachments/assets/e704d4c4-58d9-463b-905e-c347f43a35cb" />
Alertas registradas por Suricata durante el proceso de monitoreo. 
<img width="903" height="508" alt="{248D8831-EB13-4288-A8F2-654285021331}" src="https://github.com/user-attachments/assets/079853c6-aafe-4a1e-b9db-79fd75df1544" />
<img width="902" height="74" alt="{B5FF99BA-5883-4145-9D7D-4D04FECFE8B3}" src="https://github.com/user-attachments/assets/e7f1289b-3923-4e93-9bfa-7cbe540b33f4" />
ITEM 3 IMPLEMENTACIÓN DE SIEM MEDIANTE WAZUH 
<img width="903" height="508" alt="{F396D463-DE22-4C28-A5CD-2D54368B9ED7}" src="https://github.com/user-attachments/assets/620571ed-52e1-40e2-bef8-38b59cde56c1" />
<img width="903" height="508" alt="{3670A3A1-3AA0-4B0D-9D32-42A8B98CCBA6}" src="https://github.com/user-attachments/assets/3e91ffb0-8527-45bf-9a23-315ee337dc27" />
<img width="486" height="785" alt="{9A6D9522-0BDD-4F5D-8123-B7B85BE1CB41}" src="https://github.com/user-attachments/assets/41a4360f-9351-4d47-ad97-89c5458abdf6" />
<img width="900" height="506" alt="{5575AC29-3645-4CA5-9BD0-3D7330B4D7FC}" src="https://github.com/user-attachments/assets/ebd1d221-3991-4afa-b779-8678ca4f537b" />
<img width="900" height="509" alt="{D9433389-471F-4076-AB40-E405D1E07A94}" src="https://github.com/user-attachments/assets/92f0853f-0739-4938-be30-0e626fa37115" />
<img width="902" height="505" alt="{E11DFF77-8EDC-4C0E-AC82-120FC866CF8D}" src="https://github.com/user-attachments/assets/d520245f-d7eb-48ef-b8e9-d9d8878ce899" />
<img width="902" height="508" alt="{C0D4DDE0-B46B-41A2-A5C2-98A9786ACB4D}" src="https://github.com/user-attachments/assets/6e183e00-e660-49ae-80af-b6ef79e19d6a" />
<img width="902" height="508" alt="{FE365E12-4830-4585-B227-A1656DB5173A}" src="https://github.com/user-attachments/assets/6d893909-1e98-4f18-b90f-faa01779c1cf" />
<img width="903" height="506" alt="{6C5F3F66-F99A-4197-AF5E-7975FCCB2FEA}" src="https://github.com/user-attachments/assets/42895ff8-3439-4ee7-9f9f-3e8f83567138" />
<img width="905" height="508" alt="{20571FA6-A552-43CE-B9BE-EEFC37853C8C}" src="https://github.com/user-attachments/assets/da5f6305-4dd0-4157-bf37-3885a93e02c2" />
