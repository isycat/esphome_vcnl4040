Drop-in ESPHome library to use vs VCNL4040 light/proximity sensor.
Made for, and tested with, with Microbots.io CodeCell.

## Example Config:
```yaml
esphome:
  # ...
  libraries:
    - "SPI"
    - "Wire"
    - "Adafruit BusIO"
    - "Adafruit VCNL4040"
  
external_components:
  - source:
      type: git
      url: https://github.com/isycat/esphome_vcnl4040.git
      ref: "0.2"
    components: [vcnl4040]

vcnl4040:
  update_interval: 10s
  proximity:
    name: Proximity
  lux:
    name: Lux
  rawlight:
    name: Raw Light

```
![image](https://github.com/user-attachments/assets/1430509f-f4a8-4cae-9122-c4e741b862a0)

