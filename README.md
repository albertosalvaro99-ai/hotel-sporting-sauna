# Sauna Booking App (Hotel)

Turni:
- 16:00–17:30
- 17:40–19:10
- 19:20–20:50

Regole:
- Capienza 6 persone per turno (totale hotel).
- Max 1 prenotazione al giorno per camera.

## Setup DB (Supabase)
1) Crea un progetto Supabase
2) SQL Editor → esegui `supabase/schema.sql`
3) Table Editor → `rooms` → Import data CSV → importa `supabase/rooms_tokens.csv`

## Config
Copia `.env.example` in `.env.local` e compila:
- `SUPABASE_URL`
- `SUPABASE_SERVICE_ROLE_KEY` (solo server)
- `ADMIN_KEY` (password lunga)

## Avvio
```bash
npm install
npm run dev
```

## URL
- Ospite: `/sauna?token=...`
- Admin: `/admin` (richiede Admin Key)

Data pacchetto: 2026-01-11
