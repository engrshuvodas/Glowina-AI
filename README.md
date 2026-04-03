<div align="center">
  <h1>✨ Glowina AI</h1>
  <p><strong>Advanced AI-Powered Skincare Assistant App</strong></p>
  <p><i>Your personal dermatologist powered by blazing fast AI models.</i></p>
  
  <p>
    <img src="https://img.shields.io/badge/Version-2.2-FFB6C1?style=for-the-badge&logo=appveyor" alt="Version" />
    <img src="https://img.shields.io/badge/Flutter-%3E%3D3.0.0-02569B?style=for-the-badge&logo=flutter&logoColor=white" alt="Flutter" />
    <img src="https://img.shields.io/badge/Node.js-Backend-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js" />
    <img src="https://img.shields.io/badge/Groq-Llama_3.3_70B-orange?style=for-the-badge&logo=fastapi" alt="Groq API" />
    <img src="https://img.shields.io/badge/MongoDB-Powered-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB" />
  </p>
</div>

---

## 🚀 What's New in Version 2.2?
- **Name Transformation**: Officially transitioned from GlowAI to **Glowina AI**.
- **Integrated About System**: A dedicated central About UI inside both the Mobile and Web App (including dynamic versioning & changelog integration).
- **Intelligent Engine Switch**: Swapped out the legacy GPT-3.5 integration for the **Groq API** running precisely on the **Llama-3.3-70b-versatile** model for incredibly fast, medically-inclined AI analysis interactions.

## 🛠️ Accurate Tech Stack (Real Data)

**Frontend Application** 📱
- **Framework**: Flutter SDK (v3.0.0+)
- **Font & UI**: `google_fonts ^6.1.0`, `cupertino_icons`
- **Network & Linking**: `http ^1.1.0` and `url_launcher ^6.2.1`

**Backend Server** ⚙️
- **Runtime**: Node.js
- **Server Framework**: Express.js (`v4.18.2`)
- **Database Wrapper**: MongoDB with Mongoose (`v7.5.0`)
- **AI Integration Protocol**: OpenAI SDK (`v4.10.0`) wrapped around the **Groq Cloud API**.

## 📂 Project Structure
- `backend/`: Node.js server handling sophisticated AI mapping (JSON formatting & doctor alerts) and MongoDB connections.
- `frontend/`: Premium Flutter mobile client providing beautifully designed chat logic, symptom suggestions, and AI integrations.
- `web-preview/`: A sleek, HTML/JS/CSS interactive web mockup to test AI engine responses dynamically on the browser.

---

## 💻 Easy to Run Instructions

### 1. Backend Server Setup
1. Verify that **Node.js** and **MongoDB** are installed and running locally on your device.
2. Open your terminal and change directory to the backend setup:
   ```bash
   cd backend
   ```
3. Install package connections precisely (Express, Mongoose, OpenAI SDK):
   ```bash
   npm install
   ```
4. **Environment Variables Config:**
   - Create or open the `backend/.env` file.
   - **Crucial step**: Instead of OpenAI, we now strictly utilize Groq. Provide your **`GROQ_API_KEY`**.
   - Optional: Adjust `MONGODB_URI` mapping if you don't map to `mongodb://localhost:27017/glowina_ai`.
5. Launch your Node Server:
   ```bash
   npm start
   ```
   *The Express Router should initiate successfully on http://localhost:5000*

### 2. Frontend Mobile Setup
1. Verify the **Flutter SDK (>=3.0.0)** is initialized on your device alongside an Android Emulator/iOS Simulator.
2. Open a separate terminal and head into the frontend folder:
   ```bash
   cd frontend
   ```
3. Secure UI packages & project dependencies:
   ```bash
   flutter pub get
   ```
4. Trigger the app build:
   ```bash
   flutter run
   ```

*(Note: Under `api_service.dart`, verify that the `baseUrl` correlates with the emulator routing standard to `http://10.0.2.2:5000`. Switch it to `http://127.0.0.1:5000` or `http://localhost:5000` if validating over iOS Simulator/Web)*
