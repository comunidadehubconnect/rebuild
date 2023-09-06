 <p align="center">
<img src="https://cwmkt.com.br/wp-content/uploads/2023/08/logo-github-cwmkt.svg" alt="DispZap Whats Marketing" width="240" />
<p align="center">Seja bem-vindo ao Guia de atualização do n8n, nodejs e quepasa 🚀</p>
</p>
  
<p align="center">
<img src="https://whatsapp.com/favicon.ico" alt="WhatsAPP-logo" width="32" />
<span>Grupo WhatsaAPP: </span>
<a href="https://link.cwmkt.com.br/grupo-whats" target="_blank">Grupo</a>
</p>

<hr />
<hr />

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


  
