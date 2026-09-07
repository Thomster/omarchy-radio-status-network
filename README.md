# omarchy-radio-status-network

A drop-in replacement for the stock [Omarchy](https://omarchy.org/) network
bar widget that adds a **Disabled** state.

The stock panel only distinguishes "Ethernet", "Wi-Fi", and "Disconnected" —
so when the Wi-Fi radio is switched off and Ethernet isn't connected, it
still reads "Disconnected", the same label it uses when Wi-Fi is on but
simply not associated to a network. This clone tells the two apart: when
there's Wi-Fi hardware present, its radio is off, and no wired connection is
up, the panel reads **"Disabled"** instead.

Everything else — Wi-Fi scanning/connecting, band selection, DNS provider
switching, connection stats, QR sharing, speed test — behaves exactly like
the stock panel, since this is a clone of it with one state added.

## Install

```
omarchy plugin add https://github.com/Thomster/omarchy-radio-status-network.git
```

Installing switches the bar's network widget over to this plugin in place of
the stock one.

## Requirements

None beyond stock Omarchy.

## Related

Complements [omarchy-gsm-status](https://github.com/Thomster/omarchy-gsm-status)
(GSM bar icon) and [omarchy-network-priority](https://github.com/Thomster/omarchy-network-priority)
(Ethernet > Wi-Fi > GSM enforcement), but none of the three depend on each
other — each reads Wi-Fi/Ethernet/GSM state directly rather than through one
another.

## License

MIT
