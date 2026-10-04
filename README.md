# Tatva PaySync POS

A tablet-optimized point-of-sale and inventory tracking application built with FlutterFlow and Firebase Firestore.

## Architecture
- **Frontend UI:** FlutterFlow (Tablet Canvas)
- **Database:** Google Cloud Firestore (`asia-south1`)
- **Hosting & Digital Receipts:** Firebase Hosting (Static HTML/JS receipt generator)
- **Notifications:** Firebase Cloud Messaging / Cloud Functions for automated low-stock alerts

## SKU Format Convention
Format: `[CATEGORY]-[PRODUCT_NAME]-[SCENT/VARIANT]-[PACK_SIZE]`
Example: `CND-JAR-VAN-P01` (Candle > Jar > Vanilla > Pack of 1)


tavta-paysync-pos/
├── README.md
├── firestore.rules
├── schemas/
│   ├── products.json
│   ├── customers.json
│   └── orders.json
├── receipt-template/
│   └── index.html
└── functions/
    └── index.js
