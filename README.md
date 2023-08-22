  <p align="center">
  <img src="https://cwmkt.com.br/wp-content/uploads/2023/08/logo-github-cwmkt.svg" alt="DispZap Whats Marketing" width="240" />
  <p align="center">Seja bem-vindo ao Guia de Rebuild no chatwoot 🚀</p>
  </p>
 
  <details>
<summary>Para individualizar conversas entre agentes</summary>

```bash
mv /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue /home/chatwoot/chatwoot/app/javascript/dashboard/components/ChatList.vue.old
```

```bash
cd /home/chatwoot/chatwoot/app/javascript/dashboard/components
```

```bash
wget "https://raw.githubusercontent.com/cwmkt/quepasa/main/ChatList.vue"
```

Após alterações acima, rebuildar seu Chatwoot

```bash
sudo -i -u chatwoot
cd chatwoot
```

```bash
rake assets:precompile RAILS_ENV=production
```

```bash
exit
```

```bash
systemctl daemon-reload && systemctl restart chatwoot.target
```

</details>


  
