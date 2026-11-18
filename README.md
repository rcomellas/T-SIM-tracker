# T-SIM-tracker

Imatges i pedaços OTA del tracker T-SIM. Cada ordre OTA apunta a un commit concret.

## Obsolets (no s'han d'enviar)

- `firmware/firmware-0.3.18-basic-from-0.3.17-basic.delta` (18/11/2026): la 0.3.18 fa servir
  `AT+CBC` com a tensió de bateria, però a la placa Standard és la tensió regulada del mòdem
  (3,27 V amb la bateria a 4,08 V), i llavors rebutja totes les OTA amb `battery_low`.
  Substituïda per la 0.3.19 (projecte, commit `3aacec4`), instal·lada a sim7080_2 per USB.
