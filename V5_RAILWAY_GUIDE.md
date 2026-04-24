# TGX Bot V5 Railway

Tambahan ini tidak menghapus file lama. Railway menjalankan `node v5/safe-start.js` lewat `railway.json`.

## Fitur V5
- Anti crash handler dengan restart otomatis.
- Railway restart policy `ON_FAILURE`.
- Web panel di `/`.
- Health check di `/healthz`.
- API status di `/api/status`.
- Presence/profil bot Discord bisa diatur dari Variables.

## Variables Railway
Wajib:
```env
TOKEN=token_bot_baru
CLIENT_ID=id_aplikasi_bot
GUILD_ID=id_server
OWNER_ID=id_owner
```

Opsional untuk profil/presence bot:
```env
BOT_STATUS=online
BOT_ACTIVITY=/help | Premium V5
BOT_ACTIVITY_TYPE=Watching
BOT_NAME=TGX Bot
```

`BOT_ACTIVITY_TYPE` bisa: `Playing`, `Watching`, `Listening`, atau `Competing`.

## Deploy Command
Setelah deploy, buka Railway Shell lalu jalankan:
```bash
npm run deploy:guild
```

## Panel Web
Buka domain Railway kamu. Contoh:
```text
https://nama-project.up.railway.app/
```

## Catatan Keamanan
Jangan upload `.env` ke GitHub. Masukkan semua token lewat Railway Variables.
