# 1️⃣ Instalar Node.js e Git (se ainda não tiver)
pkg update && pkg upgrade -y
pkg install nodejs-lts git -y

# 2️⃣ Instalar serve e Expo CLI globalmente
npm install -g serve
npm install -g expo-cli

# 3️⃣ Clonar o repositório do GitHub
git clone https://github.com/SEU_USUARIO/mupe-taxi.git

# 4️⃣ Entrar na pasta do projeto
cd mupe-taxi

# 5️⃣ Rodar frontend Web (PWA)
cd web
npm install
serve public -s   # abre link para testar no navegador

# 6️⃣ Rodar backend API
cd ../api
npm install
node src/index.js  # servidor API rodando

# 7️⃣ Rodar app Mobile (Expo)
cd ../mobile
npm install
expo start         # gera QR Code para abrir no Expo Go
