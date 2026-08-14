COIN FLIP — ALL PAGES PROJECT

USER:
1 signup.html
2 login.html
3 index.html (Lobby)
4 coinflip.html
5 profile.html
6 deposit.html
7 withdrawal.html

ADMIN:
8 admin.html
9 admin-users.html
10 admin-user.html
11 admin-coins.html
12 admin-games.html
13 admin-coinflip.html
14 admin-transactions.html

FIRESTORE:
users/{uid}
coins/{coinId}
games/{gameId}
settings/{id}
deposits/{id}
withdrawals/{id}

AUTH:
Firebase Email/Password Authentication.

ADMIN SETUP:
1. Firebase Authentication me Email/Password enable karo.
2. Firestore enable karo.
3. firestore.rules deploy karo.
4. Signup se admin account banao.
5. Firestore users/{UID} me isAdmin = true (Boolean) set karo.
6. admin.html open karo.

IMPORTANT:
Ye project tumhari requested Firebase Authentication + Firestore-only architecture follow karta hai.
Cloud Functions use nahi ki gayi hain.
Balance/stats ko user profile se separate rakhne ka structure included hai, lekin Firebase-only client-side game execution ko trusted server execution ke barabar tamper-proof nahi mana ja sakta. Real-money gambling ke liye local laws/compliance aur trusted server-side execution ki zarurat hoti hai.
