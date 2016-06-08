# nfc-controller-itead-pn532-uart

This role prepares Raspberry PI to be a NFC controller for ITEAD PN532 chip based boards. This role is basically
automation of guide on https://www.raspberrypi.org/forums/viewtopic.php?f=45&t=78966.

WIKI of the hardware: http://wiki.iteadstudio.com/ITEAD_PN532_NFC_MODULE

This role presumes you have the NFC reader connected in mode and via [UART](https://electrosome.com/uart-raspberry-pi-python/).

## Requirements

After this role passes, please reboot your RPi.

## Example

Playbook file:

```yaml
---
- hosts:  raspberries
  user:   pi
  roles:
    - role:   nfc-controller-itead-pn532-uart
      tags:
        - nfc
```

Requirements file:

```yaml
---
- src: rooland-provisioning.nfc-controller-itead-pn532-uart
```

## License

BSD

## Author Information

- Usually idling on Freenode as lipoqil
- http://him.rlnd.cz
