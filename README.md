# Argentina Import Export Data MCP

**Argentina Customs Data: Importers, Suppliers & HS Codes.** Argentina import export data for your AI assistant. Search Argentina customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Argentina trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/argentina
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Argentina: the server tells your AI to filter on `AR` unless you ask about another country

## Argentina data coverage

- **Years:** 2019–2026
- **Records:** Import declarations: Argentine importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `AR` (use `buyerCountry: "AR"` for imports into Argentina)
- **Common products:** vehicle parts (HS 8708), soybeans (HS 1201), nitrogen fertilizers (HS 3102), natural gas (HS 2711)

## Notable traders in the data

Companies that appear most often in recent Argentina records (by number of declaration lines, not value):

**Importers**

- Ford Argentina
- Toyota Argentina
- Cargill
- Bunge Argentina
- Volkswagen Argentina
- Siderar (Ternium Argentina)

## Example prompts

- *"Who are the top importers of vehicle parts (HS 8708) into Argentina?"*
- *"Which suppliers ship soybeans to Cargill in Argentina?"*
- *"List Argentine importers of fertilizers (HS 3102) in 2025"*
- *"What does Toyota Argentina import, by origin country?"*
- *"Show recent import shipments for Bunge Argentina"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Argentina import data, Argentina export data, Argentina customs data, Argentina shipment data, importers in Argentina, Argentina buyers and suppliers, HS code search, datos de importación Argentina, importadores de Argentina, comercio exterior, posición arancelaria NCM
