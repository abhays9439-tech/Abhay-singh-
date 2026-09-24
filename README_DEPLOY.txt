AP Best Social Media Services Provider — Production-ready starter

1. Install Node.js 20+.
2. Put the project on a VPS/hosting service that supports Node.js.
3. Copy .env.example to .env and set a strong SESSION_SECRET, ADMIN_EMAIL and ADMIN_PASSWORD.
4. Run: npm install
5. Run: npm start
6. Put HTTPS in front of the Node server in production.
7. The supplied PhonePe QR is included as public/phonepe_qr.png.
8. Current QR flow is manual: customer pays, enters UTR, admin verifies and changes order status.
9. For automatic payment confirmation, onboard a merchant payment gateway and add its server-side API/webhook credentials. Never put secret API keys in frontend JavaScript.
10. For automatic social-service fulfillment, add only a provider/API that you are authorized to use; store its API key in server-side environment variables.

Important: the included QR image should only be used if it belongs to the business receiving the payments. The website does not automatically verify bank payments from a static QR.
