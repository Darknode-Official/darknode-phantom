# PHANTOM

Network traffic analysis and deep packet inspection platform for cybersecurity education.

Part of the [Darknode](https://darknode.ai) cybersecurity education platform.

> Screenshot coming soon

## Features

PHANTOM is a browser-based network traffic analyzer inspired by Wireshark, built entirely in vanilla JavaScript with no dependencies.

### 8 Analysis Tabs

- **Dashboard** -- Connection monitor, protocol distribution chart, top talkers, bandwidth gauge
- **Capture** -- PCAP file import and parsing, hex viewer, protocol filtering, packet search
- **Protocol Dissector** -- Layer-by-layer packet breakdown (Ethernet, IP, TCP/UDP, HTTP/DNS/TLS), interactive tree view
- **Flow Analysis** -- TCP session reconstruction, conversation pairs, data volume, state tracking
- **Anomaly Detection** -- Beaconing detection, DNS tunneling patterns, DGA domain identification, unusual port activity
- **DNS Inspector** -- Query/response log, DGA scoring, query type distribution, TTL analysis
- **TLS/SSL** -- Certificate chains, cipher suites, JA3 fingerprints
- **Statistics** -- Packet size histogram, protocol hierarchy, endpoint matrix, I/O graph

### Key Capabilities

- 50 realistic sample packets across 6 protocols (TCP, UDP, DNS, HTTP, TLS, ICMP)
- Color-coded protocol display (TCP blue, UDP green, DNS yellow, HTTP orange, TLS purple, ICMP cyan)
- Classic hex dump viewer with selectable field highlighting
- Inline CSS with full theme support (classic, pro-light, pro-dark)
- ES module with `renderPhantom(container)` and `cleanupPhantom()` exports
- Zero external dependencies

## Usage

PHANTOM is designed to run inside the Darknode web platform. It can also be imported as a standalone ES module:

```js
import { renderPhantom, cleanupPhantom } from './phantom.js';
renderPhantom(document.getElementById('app'));
```

## License

MIT -- see [LICENSE](LICENSE) for details.

---

Built by [Darknode](https://darknode.ai)
