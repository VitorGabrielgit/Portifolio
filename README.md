# 📌 Como Atualizar o Projeto e Publicá-lo no GitHub Pages

Este guia ensina como atualizar o código do projeto, fazer deploy no GitHub Pages e garantir que as mudanças fiquem disponíveis online.

---

## 🛠 **1. Clonar o Repositório (Se Necessário)**
Se você ainda não tem o projeto na sua máquina, use este comando:
```sh
git clone https://github.com/VitorGabrielgit/Portifolio.git
```
Depois, entre na pasta do projeto:
```sh
cd Portifolio
```

---

## 🔄 **2. Atualizar o Código**

### 2.1. Atualizar Dependências (Se Necessário)
Antes de começar, certifique-se de que todas as dependências estão atualizadas:
```sh
npm install
```

### 2.2. Fazer as Mudanças no Código
Edite os arquivos conforme necessário (HTML, CSS, JS, componentes, etc.).

### 2.3. Testar o Projeto Localmente
Antes de publicar, verifique se o projeto está funcionando corretamente:
```sh
npm start
```
Abra o navegador e acesse `http://localhost:3000/` para testar.

---

## 🚀 **3. Fazer Deploy no GitHub Pages**
Após as mudanças, siga os passos abaixo para publicar no GitHub Pages:

### 3.1. Gerar os arquivos de produção
```sh
npm run build
```
Isso cria a pasta `build/` com os arquivos otimizados.

### 3.2. Enviar para o GitHub Pages
```sh
npm run deploy
```
Isso publicará automaticamente o projeto no GitHub Pages.

---

## ✅ **4. Confirmar a Atualização**
Após o deploy, abra o navegador e acesse o link do GitHub Pages para ver as mudanças aplicadas:
```
https://vitorgabrielgit.github.io/Portifolio/
```
Se a atualização não aparecer imediatamente, tente limpar o cache do navegador (`Ctrl + Shift + R`).

---

## ⚠ **Erros Comuns e Soluções**

### ❌ **Erro 403 ao tentar enviar mudanças**
Se o erro indicar "Permission Denied" ao tentar enviar mudanças para o repositório:
```sh
git remote remove origin
```
Depois, adicione o repositório novamente com seu usuário:
```sh
git remote add origin https://github.com/VitorGabrielgit/Portifolio.git
```

### ❌ **Mudanças não aparecem no GitHub Pages**
- Aguarde alguns minutos, pois pode levar um tempo para atualizar.
- Force a atualização no navegador (`Ctrl + Shift + R`).
- Confirme se o branch `gh-pages` foi atualizado corretamente.

---

## 🔄 **5. Atualizar o Código no GitHub (Opcional)**
Se quiser atualizar o repositório com as mudanças locais:
```sh
git add .
git commit -m "Atualização do portfólio"
git push origin main
```

Isso manterá o repositório Git sempre atualizado com as últimas alterações do projeto.

---

## 📌 **Pronto!**
Agora você já sabe como atualizar e publicar o projeto corretamente! 🚀🎉
