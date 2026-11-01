# India Land Parcels & Khasra Lookup MCP (भारत)

[हिन्दी](#हिन्दी)

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Indian land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- Cadastral parcels from five states' land-record portals, compiled by datameet: Rajasthan (Rajdharaa), Madhya Pradesh (MPBhulekh), Goa (OneMapGoaGIS), Assam (Bhuvan) and Lakshadweep
- Parcel lookup by coordinates, Madhya Pradesh ULPIN, or khasra/survey number in its village (`35/1` in Calem, Goa)
- Each state's own fields: village, tehsil and district codes, survey and subdivision numbers, land-type codes
- Satellite and street map images of a parcel and its neighbours, labelled by khasra or survey number

Only these five states are loaded. The maps are digitised village sheets: offsets of 10 m or more from imagery are common. Goa's occupant names are left out.

## Connect

```
https://bumiatlas.com/mcp/india
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/india](https://bumiatlas.com/mcp-docs/india).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `IN_parcel_search` | Find parcels by `latitude, longitude`, ULPIN, or khasra/survey number with state and village; each result is the whole record, the boundary as GeoJSON on request |
| `IN_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its khasra or survey number |

## Example prompts

- *"Which parcel is at 15.34334, 74.17635 in Goa?"*
- *"Find survey number 35/1 in Calem, Goa, and show it on satellite imagery."*
- *"List the parcels of a village in Rajasthan."*
- *"Show the khasra parcels around this point."*

## Data source

Parcels from the state land-record portals (Rajdharaa, MPBhulekh, OneMapGoaGIS, Bhuvan, Bharatmaps), compiled by datameet / ramSeraph indian_cadastrals (CC0). A copy of public data for research, not a legal land record.

## हिन्दी

अपने AI सहायक (Claude, ChatGPT या Cursor) को Model Context Protocol (MCP) के ज़रिए [BumiAtlas](https://bumiatlas.com) से जोड़ें और भारत के भूमि अभिलेखों पर शोध करें।

- राजस्थान, मध्य प्रदेश, गोवा, असम और लक्षद्वीप के भू-खंड
- निर्देशांक, ULPIN या गाँव में खसरा/सर्वे नंबर से खोज
- भू-खंड और उसके पड़ोसी खंडों की सैटेलाइट और मानचित्र तस्वीरें

मालिकों के नाम शामिल नहीं हैं।

**जोड़ें:** किसी भी MCP क्लाइंट में `https://bumiatlas.com/mcp/india` को custom connector के रूप में जोड़ें और Google से साइन इन करें। टूल के नाम अंग्रेज़ी में हैं, लेकिन सहायक हिन्दी में जवाब दे सकता है।
