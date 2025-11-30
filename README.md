# 🏛️ Al Karam Digital Revenue & Land Records Portal

Yeh ek modern, responsive web application hai, jise zameen (land) aur raajswa (revenue) records ko digital roop se dekhne aur verify karne ke liye banaya gaya hai. Yeh portal **Tailwind CSS** aur **Lucide Icons** ka upyog karta hai aur backend data handling ke liye **Firebase Firestore** ka prayog karta hai.

## ✨ Mukhya Visheshtaayein (Key Features)

* **Khasra/Plot ID Search:** Khasra ID daalkar turant zameen ka official record dekhein.
* **Mock Data Seeding:** Shuruat mein, kuch sample records (1025, 2078, 3500) Firebase mein seed kiye jaate hain.
* **Quick Services Links:** Zaruri Google Drive folders ke liye direct links (Revenue Record, Personal Gallery, Agreements).
* **Modern UI:** Dark theme, responsive design ke liye Tailwind CSS ka istemaal.

## 🛠️ Technology Stack

* **Frontend:** HTML5, JavaScript
* **Styling:** Tailwind CSS (CDN)
* **Icons:** Lucide Icons (CDN)
* **Backend/Database:** Firebase Firestore & Firebase Auth (Anonymous Sign-in for public access)

## 🚀 Setup aur Deployment

Yeh project ek single HTML file hai, isliye iska deployment bahut aasan hai.

### Local Setup

1.  **Clone the repository:**
    ```bash
    git clone [AAPKI REPO LINK HERE]
    ```
2.  **Open `index.html`:** Bas file ko apne web browser mein open karein.

### Firebase Integration (Zaroori Kadam)

Search function ko theek se kaam karne ke liye, aapko **Firebase** setup karna hoga.

1.  **Firebase Project Banayein:** Firebase console mein ek naya project banayein.
2.  **Web App Add Karein:** Project mein ek web app register karein aur uska `firebaseConfig` note karein.
3.  **Authentication Enable Karein:** Auth tab mein jaakar **Anonymous** sign-in method enable karein.
4.  **Firestore Data:**
    * Firestore Database banayein.
    * `index.html` file mein `seedMockData()` function data seed karta hai. Jab aap pehli baar page load karenge, toh yeh mock data automatically database mein create ho jayega (Collection: `artifacts/{appId}/public/data/land_records`).

### GitHub Pages Deployment

Aap is portal ko turant live kar sakte hain:

1.  **GitHub Repo Banayein:** Apne GitHub account par ek naya repository banaein.
2.  **Files Upload Karein:** `index.html` aur `README.md` files ko upload karein.
3.  **Deploy Karein:** Repository Settings mein jaakar **Pages** section mein jayein aur Source Branch ko `main` ya `master` (root directory) set karein. GitHub Pages aapka portal turant deploy kar dega.
