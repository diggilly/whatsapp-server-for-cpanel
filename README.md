# whatsapp-server-for-cpanel
integrate a whatsapp nodejs server on cpanel in less that a minute

## whatsapp nodejs structure 
```
/home3/nyumban9/app.onhandi.com/node-engine/
├── .env                      # ✅ Configured & Working
├── .gitignore                # ✅ Set
├── package.json              # ✅ Dependencies Installed
├── server.js                 # ✅ Entry Point (Running on Port 3000)
│
├── src/
│   ├── config.js             # ✅ App Configuration
│   ├── db.js                 # ✅ MySQL Pool Connection
│   │
│   ├── controllers/
│   │   └── WhatsAppController.js  # ✅ Manages Sockets, QR, Connections
│   │
│   ├── routes/
│   │   └── api.js            # ✅ API Endpoints (/sessions, /messages)
│   │
│   ├── services/
│   │   ├── ConnectionService.js   # ✅ Handles QR Logic, Reconnects, DB Updates
│   │   └── MessageService.js      # ⏳ EMPTY (Our Next Target!)
│   │
│   ├── utils/
│   │   └── whatsappHelper.js      # ✅ Helper functions (Check Number, Send)
│   │
│   └── ... (other folders as needed)
│
├── sessions/                 # 💾 Stores Auth Credentials (Auto-created)
└── logs/                     # 📝 Logs

```
