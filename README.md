# IT Platforms Tracker

Team website: sab platforms ki list, tick "Done", notes, aur "Our platform" tab.
Database: Supabase (free). Hosting: Vercel (free). Code: GitHub.

## Step 1: Pehle test karo (2 minute)
`index.html` ko double-click karke browser mein kholo. Ye "Demo mode" mein chalega
(data sirf aapke device par). Isse aap design dekh sakte ho.

## Step 2: Database banao (Supabase)
1. supabase.com par jao, free account banao, **New project** dabao (naam: it-tracker).
2. Left menu: **SQL Editor** > **New query**.
3. `supabase-setup.sql` ki poori file copy karke paste karo aur **Run** dabao. (Sirf ek baar.)
4. Left menu: **Project Settings** > **API**. Wahan se 2 cheezein copy karo:
   - **Project URL**
   - **anon public** key
5. `config.js` kholo aur dono yahan paste karo:
   ```js
   window.APP_CONFIG = {
     SUPABASE_URL: "https://xxxx.supabase.co",
     SUPABASE_ANON_KEY: "eyJ...."
   };
   ```

## Step 3: GitHub par upload karo
1. github.com par new repository banao (naam: it-platforms-tracker).
2. **Add file > Upload files** se in files upload karo: `index.html`, `config.js`, `vercel.json`
   (`supabase-setup.sql` aur `README.md` bhi daal sakte ho). **Commit** karo.

## Step 4: Vercel par deploy karo
1. vercel.com par GitHub se login karo.
2. **Add New > Project**, apni repository select karo, **Import**.
3. Framework Preset: **Other**. Build command aur Output folder khali chhor do. **Deploy** dabao.
4. Vercel aapko link dega (jaise `it-platforms-tracker.vercel.app`). Ye link team ko bhej do.

## Kaise use karna hai
- Pehli baar website khuli to apna naam chuno (Hamad, Irfan, Hanzala, Adnan).
- Platform ke card par tick dabao = Done. Sab ko foran dikhega.
- **Notes** se "Services we found" aur "How we can be different" likho (khud save hota hai).
- **Add platform** se naya platform add karo.
- **Our platform** tab: apni banayi hui platform ka naam, link aur ideas yahan likho.

## Zaroori baat
Is website mein login nahi hai. Jis ke paas link hoga wo edit kar sakta hai.
Link sirf team ko do. Platforms ke URLs ek baar khud check kar lena.
